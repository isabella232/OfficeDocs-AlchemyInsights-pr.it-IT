---
title: Problemi di connessione SSO
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/21/2021
ms.locfileid: "49918141"
---
# <a name="sso-connection-issues"></a>Problemi di connessione SSO

1. Seguire [Avvio rapido: guida alla configurazione delle proprietà di un'applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) per configurare l'applicazione.
2. A seconda dell'applicazione e dell'opzione [Single #A0](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) scelta, seguire le indicazioni appropriate riportate di seguito:
    - Per configurare **un'applicazione** locale per l'accesso Single #A0 basato su **SAML,** vedere Single #A0 SAML per le applicazioni locali [con proxy di applicazione.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Per configurare **un'applicazione cloud** **per l'accesso Single #A0** basato su password, vedere Configurare l'accesso Single [#A0 per le password.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Per configurare **un'applicazione** locale per **l'accesso Single #A0** tramite proxy applicazione, vedere Password [vaulting for single sign-on with Application Proxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Risoluzione dei problemi relativi** al proxy di applicazione: è consigliabile iniziare a esaminare il flusso di risoluzione dei problemi, eseguire il debug dei problemi del connettore [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)dell'applicazione per determinare se i connettori proxy di applicazione sono configurati correttamente. Se si verificano ancora problemi di connessione all'applicazione, seguire il flusso di risoluzione dei problemi in [Debug Application Proxy application application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). È possibile identificare [i problemi CORS utilizzando](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) gli strumenti di debug del browser:
    - Avviare il browser e sfogliare l'App Web.
    - Premere **F12** per visualizzare la console di debug.
    - Provare a riprodurre la transazione ed esaminare il messaggio della console. Una violazione CORS produce un errore console in merito all'origine.
    - Alcuni problemi cors non possono essere risolti, ad esempio quando l'app reindirizza login.microsoft.com l'autenticazione e il token di accesso scade. La chiamata CORS non riesce. Come soluzione alternativa a questo scenario, estendere la durata del token di accesso per evitare che scada durante una sessione utente. Per ulteriori informazioni su come fare, vedere [Durate dei token configurabili in Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Risoluzione dei problemi relativi all'accesso Single #A0 basato su **SAML:** è consigliabile selezionare Problemi di accesso alle app configurate per l'accesso [Single #A0](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)basato su SAML per individuare le soluzioni ai problemi più probabili.
5. Risoluzione dei problemi relativi all'accesso Single #A0 basato su **password:** è consigliabile selezionare Risoluzione dei problemi relativi all'accesso [Single #A0 basato](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)su password in Azure AD per trovare le soluzioni ai problemi più probabili.
6. Per i problemi di connessione durante l'uso di una VPN, vedere Come usare single [sign-on (SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)su VPN e Wi-Fi connessioni.
