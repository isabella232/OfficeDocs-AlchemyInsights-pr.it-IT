---
title: Problemi relativi ai token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/20/2021
ms.locfileid: "49912039"
---
# <a name="issues-with-tokens"></a>Problemi relativi ai token

Per la risoluzione dei problemi relativi ai token, è possibile eseguire le procedure seguenti:

1. È possibile specificare la durata di token di accesso, ID o SAML emessi da Microsoft Identity Platform. Inoltre, è possibile impostare la durata dei token per tutte le app all'interno dell'organizzazione, per un'applicazione multi-tenant (più organizzazioni) o per un'entità servizio specifica all'interno dell'organizzazione. Per altre informazioni, vedere [Durata dei token configurabile in Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. I token di accesso consentono ai client di chiamare in modo sicuro le API Web protette, che li utilizzano per eseguire le operazioni di autenticazione e autorizzazione. In base alla specifica OAuth, i token di accesso sono stringhe opache senza un formato impostato. Alcuni provider di identità (IDP) usano i GUID, altri usano BLOB crittografati. Microsoft Identity Platform usa un’ampia gamma di formati di token di accesso, a seconda della configurazione dell'API che accetta il token. Per informazioni su come l'API convalida e usa le attestazioni all'interno di un token di accesso, vedere [Token di accesso di Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. La libreria di autenticazione Microsoft (MSAL) supporta diversi flussi di autenticazione per l'uso in differenti scenari di applicazioni. Per altre informazioni, vedere [Flussi di autenticazione](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. La concessione del codice di autorizzazione OAuth 2.0 può essere usata nelle app installate in un dispositivo per accedere a risorse protette, ad esempio le API Web. Tramite l'implementazione Microsoft Identity Platform di OAuth 2.0, è possibile aggiungere l'accesso, anche API, alle app per dispositivi mobili e desktop. Vedere [Flusso del codice di autorizzazione OAuth 2.0 e Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) per informazioni su come programmare direttamente nel protocollo dell'applicazione, usando qualsiasi lingua.
5. OpenID Connect (OIDC) è un protocollo di autenticazione basato su OAuth 2.0 da usare per fare in modo che un utente acceda in modo sicuro a un'applicazione. Tramite l'implementazione dell’endpoint di Microsoft Identity Platform di OpenID Connect, è possibile aggiungere l'accesso, anche API, alle app. [Microsoft Identity Platform e il protocollo OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) illustrano come eseguire questa operazione indipendentemente dalla lingua e come inviare e ricevere messaggi HTTP senza usare raccolte open source Microsoft.
    - L'endpoint UserInfo fa parte dello standard OIDC, progettato per restituire attestazioni sull'utente autenticato. Per altre informazioni, vedere [Endpoint UserInfo di Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - L'esempio [Chiamata di una Web API in un'app Web con Azure AD e OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) illustra come creare un'applicazione Web MVC che utilizza Azure AD per l'accesso tramite il protocollo OpenID Connect e come chiamare un'API Web con l'identità dell'utente connesso con i token ottenuti tramite OAuth 2.0. Questo esempio usa il middleware OWIN .NET per OpenID Connect e ADAL .NET.
6. [Configurare un'applicazione per esporre un’API Web](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis): in questa guida introduttiva si registra un'API Web con Microsoft Identity Platform e la si espone alle app client aggiungendo un ambito di esempio. Registrando l'API Web ed esponendola negli ambiti, è possibile fornire l'accesso basato sulle autorizzazioni alle relative risorse agli utenti autorizzati e alle app client che accedono all'API.
7. In Azure Active Directory B2C (Azure AD B2C), il flusso delle credenziali password del proprietario della risorsa (ROPC) è un flusso di autenticazione standard OAuth. In questo flusso un'applicazione nota anche come relying party, scambia credenziali valide con token. Le credenziali includono un ID utente e una password. I token restituiti consistono in un token ID, un token di accesso e un token di aggiornamento. Per altre informazioni, vedere [Configurare un flusso di credenziali password del proprietario della risorsa in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

