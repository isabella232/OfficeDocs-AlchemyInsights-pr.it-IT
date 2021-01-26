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
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976916"
---
# <a name="application-errors"></a>Errori dell'applicazione

Per informazioni sui codici di **errore di AADSTS** restituiti dal servizio token di sicurezza (STS) di Azure Active Directory (Azure ad)? Leggere i [codici di errore per l'autenticazione e l'autorizzazione di Azure ad](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) per individuare le descrizioni degli errori di AADSTS, le correzioni e alcune soluzioni alternative consigliate.

Gli errori di autorizzazione possono essere causati da diversi problemi, la maggior parte dei quali genera un errore 401 o 403. Ad esempio, i seguenti elementi possono portare a errori di autorizzazione:

- [Flussi di acquisizione di token di accesso](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) non corretti 
- [Ambiti di autorizzazione](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurati 
- Mancanza di [consenso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Per risolvere gli errori di autorizzazione comuni, provare a eseguire i passaggi riportati di seguito che corrispondono più fedelmente all'errore che si sta ricevendo. È possibile applicare più di uno.

**401 errore non autorizzato: il token è valido?**

Verificare che l'applicazione presenti un token di accesso valido a Microsoft Graph come parte della richiesta. Questo errore indica spesso che il token di accesso potrebbe mancare nell'intestazione della richiesta di autenticazione HTTP oppure che il token non è valido o è scaduto. È consigliabile utilizzare la [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) per l'acquisizione dei token di accesso. Questo errore può inoltre verificarsi se si tenta di utilizzare un token di accesso delegato concesso a un account Microsoft personale per accedere a un'API che supporta solo gli account di lavoro o dell'Istituto di istruzione (account organizzativi).

**403 errore non consentito: si è scelto il set di autorizzazioni appropriato?**

Controllare di aver richiesto il set corretto di autorizzazioni in base alle API di Microsoft Graph chiamate dall'app. Le autorizzazioni meno privilegiate consigliate vengono fornite in tutti gli argomenti del metodo di riferimento dell'API di Microsoft Graph. Inoltre, tali autorizzazioni devono essere concesse all'applicazione da un utente o da un amministratore. La concessione di autorizzazioni avviene normalmente tramite una pagina di consenso o concedendo le autorizzazioni utilizzando il Blade di registrazione dell'applicazione portale di Azure. Dal pannello **Impostazioni** per l'applicazione, fare clic su **autorizzazioni necessarie**, quindi fare clic su **Concedi autorizzazioni**.

- [Autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Informazioni sulle autorizzazioni e sul consenso di Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 errore non consentito: l'app ha acquisito un token per soddisfare le autorizzazioni selezionate?**

Verificare che il tipo di autorizzazioni richieste o concesse corrisponda al tipo di token di accesso acquisito dall'app. È possibile che si richiedano e si concessino le autorizzazioni per l'applicazione, ma che si utilizzino token di flusso di codice interattivo delegati invece dei token di flusso di credenziali client o che si richiedano autorizzazioni delegate ma che utilizzino token di flusso di codice delegati.

- [Ottenere l'accesso per conto di utenti e autorizzazioni delegate](https://docs.microsoft.com/graph/auth_v2_user) 
- [Flusso del codice di autorizzazione di Azure AD v 2.0-OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Ottenere l'accesso senza un utente (servizio daemon) e le autorizzazioni per l'applicazione](https://docs.microsoft.com/graph/auth_v2_service) 
- [Flusso delle credenziali client di Azure AD v 2.0-OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 errore non consentito: reimpostazione della password**

Attualmente, non sono disponibili autorizzazioni di servizio per il daemon di autorizzazioni per l'applicazione che consentono di reimpostare le password degli utenti. Queste API sono supportate solo mediante flussi di codice delegati interattivi con un amministratore connesso.

- [Autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 Forbidden: l'utente ha accesso e ha una licenza?**

Per i flussi di codice delegati, Microsoft Graph valuta se la richiesta è consentita in base alle autorizzazioni concesse all'app e alle autorizzazioni che l'utente ha eseguito l'accesso. In genere, questo errore indica che l'utente non è sufficientemente privilegiato per eseguire la richiesta o che l'utente non dispone di una licenza per i dati a cui si accede. Solo gli utenti che dispongono delle autorizzazioni o delle licenze necessarie possono eseguire correttamente la richiesta.

**403 Forbidden: è stata selezionata l'API delle risorse corretta?**

I servizi API come Microsoft Graph verificano che l'attestazione AUD (gruppo di destinatari) nel token di accesso ricevuto corrisponda al valore previsto per se stesso e, in caso contrario, genera un errore 403 Forbidden. Un errore comune risultante da questo errore consiste nel tentativo di utilizzare un token acquisito per API di Azure AD Graph, API di Outlook o API di SharePoint/OneDrive per chiamare Microsoft Graph (o viceversa). Verificare che la risorsa (o ambito) dell'app acquisisca un token per la corrispondenza con l'API chiamata dall'app.

**400 Bad Request o 403 Forbidden: l'utente è conforme ai criteri di accesso condizionale (CA) dell'organizzazione?**

In base ai criteri della CA dell'organizzazione, un utente che accede alle risorse di Microsoft Graph tramite l'app può essere messo in discussione per ulteriori informazioni che non sono presenti nel token di accesso acquistato originariamente dall'app. In questo caso, l'app riceve un 400 con un *interaction_required* errore durante l'acquisizione di un token di accesso o un 403 con *insufficient_claims* errore durante la chiamata a Microsoft Graph. In entrambi i casi, la risposta di errore contiene informazioni aggiuntive che possono essere presentate all'endpoint autorizza per contestare l'utente per ulteriori informazioni, ad esempio l'autenticazione a più fattori o la registrazione dei dispositivi.

- [Gestione delle sfide di accesso condizionale tramite MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Guida per gli sviluppatori per l'accesso condizionale di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
