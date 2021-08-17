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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084350"
---
# <a name="sso-connection-issues"></a>Problemi di connessione SSO

1. Seguire [Avvio rapido: guida alla configurazione delle proprietà di un'applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) per configurare l'applicazione.
2. A seconda dell'applicazione e [dell'opzione Single #A0](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) scelta, seguire le indicazioni appropriate di seguito:
    - Per configurare **un'applicazione** locale per il **single sign-on** basato su SAML, vedere Single #A0 SAML per le applicazioni [locali con proxy di applicazione.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Per configurare **un'applicazione cloud** per single **sign-on** basato su password, vedere [Configure password single sign-on.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Per configurare **un'applicazione** locale per **l'accesso Single #A0 tramite proxy** applicazione, vedere Password [vaulting for single sign-on with Application Proxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Risoluzione dei problemi relativi al proxy** di applicazione : è consigliabile iniziare esaminando il flusso di risoluzione dei problemi, Debug application Proxy Connector [issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), per determinare se i connettori proxy di applicazione sono configurati correttamente. Se si verificano ancora problemi di connessione all'applicazione, seguire il flusso di risoluzione dei problemi in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). È possibile identificare [i problemi cors utilizzando](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) gli strumenti di debug del browser:
    - Avviare il browser e sfogliare l'App Web.
    - Premere **F12** per visualizzare la console di debug.
    - Provare a riprodurre la transazione ed esaminare il messaggio della console. Una violazione CORS produce un errore console in merito all'origine.
    - Alcuni problemi cors non possono essere risolti, ad esempio quando l'app reindirizza a login.microsoft.com per l'autenticazione e il token di accesso scade. La chiamata CORS ha quindi esito negativo. Come soluzione alternativa a questo scenario, estendere la durata del token di accesso per evitare che scada durante una sessione utente. Per ulteriori informazioni su come fare, vedere [Durate dei token configurabili in Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Risoluzione dei problemi relativi al **single sign-on** basato su SAML: è consigliabile selezionare Problemi di accesso alle app configurate per l'accesso [Single #A0](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)basate su SAML per trovare le soluzioni ai problemi più probabili.
5. Risoluzione dei problemi relativi al **single sign-on** basato su password: è consigliabile controllare Risoluzione dei problemi di single [sign-on basato](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)su password in Azure AD per trovare le soluzioni ai problemi più probabili.
6. Per i problemi di connessione durante l'uso di una VPN, vedere Come usare single [sign-on (SSO)](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)su VPN e Wi-Fi connessioni .
