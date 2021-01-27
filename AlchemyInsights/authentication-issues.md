---
title: Problemi di autenticazione
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976853"
---
# <a name="authentication-issues"></a>Problemi di autenticazione

**Si desidera ricevere altre informazioni sui codici errore AADSTS restituiti dal servizio token di sicurezza di Azure Active Directory (Azure AD)?** Vedere [Autenticazione di Azure AD e codici di errore di autenticazione](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) per trovare la descrizione degli errori AADSTS, le correzioni e alcune soluzioni alternative suggerite.

Gli errori di autorizzazione possono essere il risultato di numerosi problemi di diversa natura, la maggior parte dei quali generano un errore 401 o 403. Ad esempio, i problemi seguenti possono causare errori di autorizzazione:

- [Flussi di acquisizione di token di accesso](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) non corretti 
- [Ambiti di autorizzazione](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) non configurati correttamente 
- Mancanza di [consenso](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Per risolvere gli errori di autorizzazione più comuni, provare tra le procedure descritte di seguito quelle che più si adattano agli errori ricevuti. È possibile che più di una procedura sia idonea all’errore ricevuto.

**Errore 401 Non autorizzato: il token è valido?**

Verificare che l'app disponga nella richiesta di un token di accesso valido a Microsoft Graph. Questo errore spesso indica che il token di accesso potrebbe non essere presente nell'intestazione della richiesta di autenticazione HTTP o che il token non è valido o è scaduto. Si consiglia vivamente di usare MSAL (Microsoft Authentication Library) per l'acquisizione di token di accesso. Inoltre, l’errore può verificarsi quando si prova a usare un token di accesso con delega concesso a un account Microsoft personale per accedere a un'API che supporta solo gli account aziendali o dell'istituto di istruzione (account dell’organizzazione).

**Errore 403 Accesso negato: si è scelto il set di autorizzazioni corretto?**

Verificare di aver richiesto il set di autorizzazioni corretto basato sulle API di Microsoft Graph chiamate dall’app. Le autorizzazioni con privilegi minimi consigliate sono disponibili negli argomenti sui metodi di riferimento delle API di Microsoft Graph. Inoltre, tali autorizzazioni devono essere concesse all'applicazione da un utente o un amministratore. La concessione delle autorizzazioni avviene in genere tramite una pagina di consenso o l'utilizzo del pannello di registrazione dell'applicazione nel portale di Azure. Nel pannello **Impostazioni** dell'applicazione, fare clic su **Autorizzazioni necessarie**, poi su **Concedi autorizzazioni**. Per altre informazioni, vedere:

- [Autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Informazioni sulle autorizzazioni e il consenso di Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Errore 403 Accesso negato: l'app ha acquisito un token corrispondente alle autorizzazioni scelte?**

Verificare che i tipi di autorizzazione richiesti o concessi corrispondano al tipo di token di accesso acquisito dall'app. Potrebbe essere necessario chiedere e concedere autorizzazioni per le app, ma usando token di flusso di codice interattivi con delega anziché token di flusso di credenziali client oppure chiedere e concedere autorizzazioni con delega, ma usando token di flusso di credenziali client anziché di token di flusso di codice con delega.

Per altre informazioni relative all’acquisizione dei token, vedere:

- [Ottenere l'accesso per conto degli utenti e autorizzazioni delegate](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - Flusso del codice di autorizzazione OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Ottenere l'accesso senza le autorizzazioni dell’utente (servizio daemon) e dell'applicazione](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - Flusso delle credenziali del client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Errore 403 Accesso negato: reimpostazione della password**

Al momento non esistono autorizzazioni da servizio a servizio daemon di autorizzazione dell‘applicazione che consentono la reimpostazione delle password degli utenti. Queste API sono supportate solo tramite flussi di codice con delega interattivi con un amministratore connesso. Per altre informazioni, vedere [Autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 Accesso negato: l'utente dispone di accesso e licenza?**

Per i flussi di codice con delega, Microsoft Graph valuta se la richiesta è stata autorizzata in base alle autorizzazioni concesse all'app e all'utente connesso. In generale, questo errore indica che l'utente non dispone di privilegi sufficienti per eseguire la richiesta **oppure** l'utente non ha una licenza per i dati a cui accede. Solo gli utenti con le autorizzazioni o le licenze necessarie possono eseguire correttamente la richiesta.

**403 Accesso negato: è stata selezionata l'API della risorsa corretta?**

I servizi API come Microsoft Graph verificano che l’attestazione *aud* (gruppo di destinatari) nel token di accesso ricevuto corrisponda al valore previsto e, in caso contrario, si verifica un errore 403 Accesso negato. Un errore comune che causa questo errore è l'uso di un token acquisito per le API Graph di Azure AD, le API di Outlook o le API di SharePoint/OneDrive per chiamare Microsoft Graph (o viceversa). Verificare che la risorsa, o l'ambito, dell'app acquisisca un token per la corrispondenza con l'API chiamata dall'app.

**400 Richiesta non valida o 403 Accesso negato: l'utente è conforme ai criteri di accesso condizionale dell'organizzazione?**

In base ai criteri di accesso condizionale di un'organizzazione, gli utenti che accedono alle risorse di Microsoft Graph tramite l'app potrebbero ricevere la richiesta di altre informazioni non presenti nel token di accesso acquisito in origine dall'app. In questo caso, l'app riceve un codice **400 con errore *interaction_required*** durante l'acquisizione del token di accesso o un codice **403 con errore *insufficient_claims*** durante la chiamata a Microsoft Graph. In entrambi i casi, la risposta di errore contiene informazioni aggiuntive che possono essere presentate all'endpoint autorizzato per richiedere all'utente altre informazioni, ad esempio l'autenticazione a più fattori o la registrazione del dispositivo.

Per altre informazioni relative all’accesso condizionale, vedere:

- [Gestione delle richieste di accesso condizionale tramite MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Indicazioni per sviluppatori relative all’accesso condizionale di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Fine del supporto per Active Directory Authentication Library (ADAL) e l'API Graph di Azure AD (AAD Graph)_* _

- A partire dal 30 giugno 2020, non verranno più aggiunte nuove funzionalità ad Active Directory Authentication Library (ADAL) e all'API Graph di Azure AD (A AD Graph). Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.
- A partire dal 30 giugno 2022, Microsoft terminerà il supporto per ADAL e Graph di AAD e non fornirà più supporto tecnico o aggiornamenti della sicurezza.
    - Le app che usano ADAL nelle versioni del sistema operativo esistenti continueranno a funzionare dopo tale data, ma non riceveranno alcun supporto tecnico o aggiornamento della sicurezza.
    - Le app che usano Graph di AAD dopo tale data potrebbero non ricevere più risposte dall'endpoint Graph di AAD.

_ *Migrazione ADAL**

È consigliabile eseguire l'aggiornamento a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), che include le funzionalità e gli aggiornamenti della sicurezza più recenti. Questo suggerimento è valido nel caso di migrazione delle applicazioni Microsoft a MSAL entro la scadenza del supporto. L'obiettivo della migrazione delle app Microsoft a MSAL è garantire che tali app possano beneficiare dei miglioramenti continui della sicurezza e funzionalità di MSAL.

- [Consultare le domande frequenti su ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Informazioni su come eseguire la migrazione delle app in base alla piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Se serve assistenza per comprendere quali app usi ADAL, è consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti (ISV) o provider di app. Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.

**Migrazione Graph di AAD**

Per le applicazioni che usano Graph di AAD, seguire le indicazioni per la [migrazione delle app Graph di AAD a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [L'elenco di controllo per la migrazione fornisce un punto di partenza](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Il portale di registrazione delle app Azure illustra quali applicazioni usano Graph di AAD. È consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti o provider di app. Il supporto Microsoft può fornire informazioni sull'utilizzo di Graph di AAD nel tenant.

 










