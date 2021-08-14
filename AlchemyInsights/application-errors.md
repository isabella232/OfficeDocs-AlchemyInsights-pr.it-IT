---
title: Errori dell'applicazione
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931453"
---
# <a name="application-errors"></a>Errori dell'applicazione

Per informazioni sui codici di errore **AADSTS** restituiti dal servizio token di sicurezza (STS) di Azure Active Directory (Azure AD)? Leggere [Autenticazione di Azure AD e i codici](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) di errore di autorizzazione per trovare descrizioni degli errori, correzioni e alcune soluzioni alternative suggerite.

Gli errori di autorizzazione possono essere il risultato di numerosi problemi di diversa natura, la maggior parte dei quali generano un errore 401 o 403. Ad esempio, quanto segue può causare errori di autorizzazione:

- [Flussi di acquisizione di token di accesso](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) non corretti 
- [Ambiti di autorizzazione](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) non configurati correttamente 
- Mancanza di [consenso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Per risolvere gli errori di autorizzazione comuni, provare la procedura riportata di seguito che corrisponde maggiormente all'errore che si sta ricevendo. Possono essere applicati più di uno.

**Errore 401 Non autorizzato: il token è valido?**

Assicurati che l'applicazione presenti un token di accesso valido a Microsoft Graph come parte della richiesta. Questo errore spesso indica che il token di accesso potrebbe non essere presente nell'intestazione della richiesta di autenticazione HTTP o che il token non è valido o è scaduto. Ti consigliamo vivamente di usare [microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) per l'acquisizione di token di accesso. Inoltre, questo errore può verificarsi se provi a usare un token di accesso delegato concesso a un account Microsoft personale per accedere a un'API che supporta solo gli account aziendali o dell'istituto di istruzione (account dell'organizzazione).

**Errore 403 Accesso negato: si è scelto il set di autorizzazioni corretto?**

Verifica di aver richiesto il set corretto di autorizzazioni in base alle API di Microsoft Graph la tua app chiama. Le autorizzazioni con privilegi minimi consigliate sono disponibili in tutti gli argomenti relativi al metodo di riferimento dell Graph API di Microsoft. Inoltre, tali autorizzazioni devono essere concesse all'applicazione da un utente o un amministratore. La concessione delle autorizzazioni avviene in genere tramite una pagina di consenso o concedendo le autorizzazioni tramite il pannello di registrazione dell'applicazione portale di Azure. Nel pannello **Impostazioni** dell'applicazione, fare clic su **Autorizzazioni necessarie**, poi su **Concedi autorizzazioni**.

- [Autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Informazioni sulle autorizzazioni e il consenso di Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Errore 403 Accesso negato: l'app ha acquisito un token corrispondente alle autorizzazioni scelte?**

Assicurati che il tipo di autorizzazioni richieste o concesse corrisponda al tipo di token di accesso acquisito dall'app. Potresti richiedere e concedere le autorizzazioni dell'applicazione, ma usando token del flusso di codice interattivo delegato anziché token del flusso di credenziali client o richiedendo e concedendo autorizzazioni delegate, ma usando i token del flusso di credenziali client anziché i token del flusso di codice delegato.

- [Ottenere l'accesso per conto degli utenti e autorizzazioni delegate](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - Flusso del codice di autorizzazione OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Ottenere l'accesso senza le autorizzazioni dell’utente (servizio daemon) e dell'applicazione](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - Flusso delle credenziali del client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Errore 403 Accesso negato: reimpostazione della password**

Al momento non esistono autorizzazioni da servizio a servizio daemon di autorizzazione dell‘applicazione che consentono la reimpostazione delle password degli utenti. Queste API sono supportate solo tramite flussi di codice con delega interattivi con un amministratore connesso.

- [Autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 Accesso negato: l'utente dispone di accesso e licenza?**

Per i flussi di codice delegato, Microsoft Graph valuta se la richiesta è consentita in base alle autorizzazioni concesse all'app e alle autorizzazioni di cui dispone l'utente connesso. In generale, questo errore indica che l'utente non dispone di privilegi sufficienti per eseguire la richiesta oppure l'utente non ha una licenza per i dati a cui accede. Solo gli utenti con le autorizzazioni o le licenze necessarie possono eseguire correttamente la richiesta.

**403 Accesso negato: è stata selezionata l'API della risorsa corretta?**

I servizi API come Microsoft Graph verificare che l'attestazione aud (gruppo di destinatari) nel token di accesso ricevuto corrisponda al valore previsto per se stesso e, in caso contrario, genera un errore 403 Accesso negato. Un errore comune che causa questo errore è l'uso di un token acquisito per le API Graph di Azure AD, le API di Outlook o le API di SharePoint/OneDrive per chiamare Microsoft Graph (o viceversa). Verificare che la risorsa, o l'ambito, dell'app acquisisca un token per la corrispondenza con l'API chiamata dall'app.

**400 Richiesta non valida o 403 Accesso negato: l'utente è conforme ai criteri di accesso condizionale dell'organizzazione?**

In base ai criteri CA di un'organizzazione, un utente che accede alle risorse di Microsoft Graph tramite l'app potrebbe essere richiesto di richiedere ulteriori informazioni che non sono presenti nel token di accesso acquisito in origine dall'app. In questo caso, l'app riceve un codice 400 con errore *interaction_required* durante l'acquisizione del token di accesso o un codice 403 con errore *insufficient_claims* durante la chiamata a Microsoft Graph. In entrambi i casi, la risposta di errore contiene informazioni aggiuntive che possono essere presentate all'endpoint di autorizzazione per la richiesta di informazioni aggiuntive all'utente (ad esempio l'autenticazione a più fattori o la registrazione del dispositivo).

- [Gestione delle sfide di accesso condizionale con MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Indicazioni per sviluppatori relative all’accesso condizionale di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
