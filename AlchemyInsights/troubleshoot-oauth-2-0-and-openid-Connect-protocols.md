---
title: Risoluzione dei problemi dei protocolli OAuth 2.0 e OpenID Connect
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898252"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Risoluzione dei problemi dei protocolli OAuth 2.0 e OpenID Connect

Per risolvere i problemi di OAuth 2.0 e OpenID Connect, eseguire i seguenti passaggi consigliati:

Fare riferimento ai seguenti articoli relativi alla configurazione e alla risoluzione dei problemi dei protocolli OAuth 2.0 e OpenID Connect:

- [Microsoft Identity Platform e flusso del codice di autorizzazione OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - Questo articolo descrive come programmare direttamente nel **flusso del codice grant (chiave di prova per code exchange)** nell'applicazione usando qualsiasi linguaggio.
- [Microsoft Identity Platform e flusso di credenziali client OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Questo articolo descrive come programmare direttamente nel **flusso delle credenziali del client** nell'applicazione.
- [Microsoft Identity Platform e credenziali di tipo password del proprietario della risorsa OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - Questo articolo descrive come programmare direttamente nel **flusso ROPC** nell'applicazione.
    - Microsoft Identity Platform supporta solo il ROPC per i tenant di Azure AD e non per gli account personali. Questo significa che è necessario usare un endpoint specifico del tenant **(https://login.microsoftonline.com/{TenantId_or_Name})** o l'endpoint delle **organizzazioni**.
    - Gli account personali che hanno ricevuto un invito per un tenant di Azure AD non possono usare ROPC.
    - Gli account senza password non possono accedere tramite ROPC. Per questo scenario, è consigliabile usare un flusso diverso per l'app.
    - Gli utenti vengono bloccati se usano l'[autenticazione a più fattori](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) per accedere all'applicazione.
    - ROPC non è supportato negli [scenari di federazione delle identità ibride](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (ad esempio, quando vengono usati Azure AD e ADFS per autenticare gli account locali). Se gli utenti vengono reindirizzati a una pagina di un provider di identità locale, Azure AD non può testare il nome utente e la password in tale provider di identità. Tuttavia, [l'autenticazione pass-through](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) è supportata con il ROPC.
    - La seguente è un'eccezione a uno scenario di federazione delle identità ibride: i criteri di individuazione dell'area di autenticazione domestica con **AllowCloudPasswordValidation** impostato su **TRUE** attiveranno il flusso ROPC per gli utenti federati quando la password locale viene sincronizzata nel cloud. Per ulteriori informazioni, consultare [Attivare l'autenticazione diretta ROPC degli utenti federati per le applicazioni legacy](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Microsoft Identity Platform e flusso On-Behalf-Of di OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - Questo articolo descrive come programmare direttamente nel **flusso On-Behalf-Of (OBO)** nell'applicazione.
- [Microsoft Identity Platform e il protocollo OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Questo articolo illustra come implementare il protocollo OpenID Connect indipendentemente dal linguaggio e descrive come inviare e ricevere messaggi HTTP senza usare raccolte open source Microsoft.

**Token di accesso**

[Token di accesso di Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Informazioni sulle modalità adottate dall'API per convalidare e usare le attestazioni in un token di accesso. Tutta la documentazione di questo articolo, tranne quanto specificato, si applica solo ai token rilasciati per le API registrate. Non si applica ai token rilasciati per le API di proprietà di Microsoft, né può essere usata per convalidare il modo in cui Microsoft Identity Platform emette i token per le API create dall'utente.

**Configurazione dell'applicazione**

[Restrizioni e limitazioni relative all'URI di reindirizzamento (URL di risposta)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - Informazioni sulla modalità di configurazione dell'URI di reindirizzamento (URL di risposta). Un URI di reindirizzamento, o URL di risposta, è la posizione in cui il server di autorizzazione invia l'utente dopo che l'app è stata autorizzata correttamente e ha concesso un codice di autorizzazione o token di accesso. Il server di autorizzazione invia il codice o token all'URI di reindirizzamento, quindi è importante registrare la posizione corretta durante il processo di registrazione dell'app.

**Provisioning delle applicazioni**

[Tutorial: sviluppare e pianificare il provisioning per un endpoint SCIM](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) - Questo articolo descrive come creare un endpoint SCIM e integrare il servizio di provisioning AAD.


