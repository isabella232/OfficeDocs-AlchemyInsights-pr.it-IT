---
title: 'Risolvere i problemi di Single #A0 (SSO) basati su password'
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
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972828"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Risolvere i problemi di Single #A0 (SSO) basati su password

Per informazioni sulle nozioni fondamentali del servizio SSO basato su password, vedere Autenticazione basata su [password con Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Configurare SSO basato su password**

1. [Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - In questo articolo vengono fornite informazioni più dettagliate sull'opzione SSO basata su password. Se l'applicazione che si sta aggiungendo richiede una configurazione personalizzata ed è necessario utilizzare SSO basato su password, questo articolo fa per te.
2. [Configurare l'accesso Single #A0](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) basato su password per le app in modalità prem- Il proxy dell'applicazione supporta diverse modalità Single Sign-On. L'accesso basato su password è destinato alle applicazioni che utilizzano una combinazione nome utente/password per l'autenticazione. Quando si configura l'accesso basato su password per l'applicazione, gli utenti devono accedere all'applicazione locale una sola volta. Successivamente, Azure Active Directory le informazioni di accesso e le fornisce automaticamente all'applicazione quando gli utenti accedono in remoto.
    - Dovresti aver già pubblicato e testato l'app con il proxy dell'applicazione. In caso contrario, seguire i passaggi descritti in [Publish applications using Azure AD Application Proxy,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) quindi continuare la configurazione del servizio SSO basato su password per le app in uso.

Per risolvere i problemi relativi al servizio SSO basato su password, vedere Risolvere i problemi relativi al [single sign-on basato su password in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
