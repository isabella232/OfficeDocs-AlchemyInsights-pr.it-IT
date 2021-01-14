---
title: Problemi con l'integrazione di SSO trasparente con le app locali
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/13/2021
ms.locfileid: "49848774"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problemi con l'integrazione di SSO trasparente con le app locali

Per risolvere i problemi relativi all'integrazione di SSO trasparente con le applicazioni locali, eseguire le operazioni seguenti:

**Passaggi consigliati**

1. Per configurare un' **applicazione locale** per il servizio **Single Sign-on tramite proxy di applicazione**, vedere [password vaulting for Single Sign-on with application proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Risoluzione dei** problemi relativi ai proxy di applicazioni: si consiglia di iniziare con la revisione del flusso di risoluzione dei problemi, di [eseguire il debug del connettore del proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)di applicazione per determinare se i connettori proxy dell'applicazione sono configurati correttamente. Se si verificano ancora problemi di connessione all'applicazione, seguire la procedura per la risoluzione dei problemi relativi all'applicazione di [debug del proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)di applicazione. È possibile [identificare i problemi di CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) utilizzando gli strumenti di debug del browser seguenti:
    1. Avviare il browser e passare all'app Web.
    1. Premere **F12** per visualizzare la console di debug.
    1. Provare a riprodurre la transazione ed esaminare il messaggio della console. Una violazione di CORS genera un errore di console relativo all'origine.
    1. Alcuni problemi di CORS non possono essere risolti, ad esempio quando l'app reindirizza a login.microsoftonline.com per l'autenticazione e il token di accesso scade. La chiamata di CORS ha esito negativo. Una soluzione alternativa per questo scenario consiste nell'estendere la durata del token di accesso, per impedirne la scadenza durante la sessione di un utente. Per ulteriori informazioni su come eseguire questa operazione, vedere [durata dei token configurabili in Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Documenti consigliati**

- [Come configurare il servizio Single Sign-on per un'applicazione proxy di applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Single Sign-On SAML per le applicazioni locali con proxy di applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Individuare e risolvere i problemi di CORS del proxy di applicazione di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Risoluzione dei problemi relativi alle configurazioni di delega vincolate Kerberos per il proxy di applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)