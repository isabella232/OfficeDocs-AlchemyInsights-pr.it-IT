---
title: Problemi relativi all'integrazione di SSO senza soluzione di continuità con le app locali
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028296"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemi relativi all'integrazione di SSO senza soluzione di continuità con le app locali

Per risolvere i problemi relativi all'integrazione di SSO senza problemi con le applicazioni locali, eseguire le operazioni seguenti:

**Passaggi consigliati**

1. Per configurare **un'applicazione** locale per **l'accesso Single #A0 tramite proxy** applicazione, vedere Password [vaulting for single sign-on with Application Proxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Risoluzione dei problemi relativi al proxy** di applicazione : è consigliabile iniziare esaminando il flusso di risoluzione dei problemi, Eseguire il debug dei problemi del connettore [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)di applicazione per determinare se i connettori proxy di applicazione sono configurati correttamente. Se persistono i problemi di connessione dell'applicazione, seguire i passaggi relativi alla risoluzione dei problemi in [Problemi relativi all'esecuzione del debug del proxy di applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). È possibile [identificare i problemi cors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) utilizzando i seguenti strumenti di debug del browser:
    1. Avviare il browser e sfogliare l'App Web.
    1. Premere **F12** per visualizzare la console di debug.
    1. Provare a riprodurre la transazione ed esaminare il messaggio della console. Una violazione CORS produce un errore console in merito all'origine.
    1. Alcuni problemi cors non possono essere risolti, ad esempio quando l'app reindirizza a login.microsoftonline.com per l'autenticazione e il token di accesso scade. La chiamata CORS ha quindi esito negativo. Come soluzione alternativa a questo scenario, estendere la durata del token di accesso per evitare che scada durante una sessione utente. Per ulteriori informazioni su come fare, vedere [Durate dei token configurabili in Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Documenti consigliati**

- [Come configurare l'accesso Single #A0 a un'applicazione proxy di applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Single #A0 SAML per le applicazioni locali con proxy di applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Comprendere e risolvere i Azure Active Directory CORS del proxy di applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Risolvere i problemi relativi alle configurazioni con delega vincolata Kerberos per il proxy di applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)