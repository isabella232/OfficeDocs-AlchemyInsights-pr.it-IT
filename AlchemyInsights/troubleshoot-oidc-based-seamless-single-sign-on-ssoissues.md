---
title: 'Risolvere i problemi di Single #A0 (SSO) basati su OIDC'
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105782"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Risolvere i problemi di Single #A0 (SSO) basati su OIDC

- Per informazioni su come aggiungere un'app basata su OIDC al tenant di Azure, vedere Guida introduttiva: Configurare single [sign-on (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)basato su OIDC per un'applicazione nel tenant di Azure Active Directory (Azure AD).
- Per ulteriori informazioni sulle app che usano lo standard OpenID Connessione per implementare il single [sign-on, vedere Understand OIDC-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Per informazioni nel caso in cui si sceglie di scrivere il codice inviando e gestendo direttamente le richieste HTTP o utilizzando una libreria open source di terze parti, anziché utilizzare una delle librerie open source, vedere [Protocolli OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)e OpenID Connessione nel Microsoft Identity Platform .

**Protocolli**

1. Microsoft Identity Platform flusso di concessione [implicito](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) - La caratteristica di definizione della concessione implicita è che i token (token ID o token di accesso) vengono restituiti direttamente dall'endpoint /authorize anziché dall'endpoint /token. Questo viene spesso usato come parte del flusso del codice di autorizzazione, in quello che viene chiamato **"flusso ibrido",** il recupero del token ID nella richiesta /authorize insieme a un codice di autorizzazione. Questo articolo descrive come programmare direttamente rispetto al protocollo nell'applicazione per richiedere token da Azure AD.
2. flusso del codice di autorizzazione [di Microsoft Identity Platform e OAuth 2.0-](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) La concessione del codice di autorizzazione OAuth 2.0 può essere usata nelle app installate in un dispositivo per ottenere l'accesso alle risorse protette, ad esempio le API Web. Usando l'Microsoft Identity Platform di OAuth 2.0, puoi aggiungere l'accesso e l'accesso api alle app per dispositivi mobili **e desktop.** In questo articolo viene descritto come programmare direttamente in base al protocollo dell'applicazione utilizzando qualsiasi linguaggio.
3. [Microsoft Identity Platform e OpenID Connessione protocollo](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Quando usi l'implementazione del Microsoft Identity Platform di OpenID Connessione, puoi aggiungere l'accesso e l'accesso api alle tue app. In questo articolo viene illustrato come eseguire questa operazione indipendentemente dal linguaggio e viene descritto come inviare e ricevere messaggi HTTP senza utilizzare librerie **open source Microsoft.**
4. flusso di credenziali [client Microsoft Identity Platform e OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - È possibile utilizzare la concessione delle credenziali client OAuth 2.0 specificata in RFC 6749, talvolta denominata **OAuth** a due vie, per accedere alle risorse ospitate sul Web utilizzando l'identità di un'applicazione. Questo tipo di concessione viene comunemente usato per le interazioni da server a server che devono essere eseguite in background, senza un'interazione immediata con un utente. Questi tipi di applicazioni vengono spesso definiti **daemon o** **account di servizio.** In questo articolo viene descritto come programmare direttamente in base al protocollo nell'applicazione.
