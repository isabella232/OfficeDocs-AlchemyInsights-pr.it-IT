---
title: "Risolvere i problemi relativi all'accesso Single #A0 basato su password"
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709497"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Risolvere i problemi relativi all'accesso Single #A0 (SSO) basato su password

Per informazioni sui concetti fondamentali di SSO basato su password, vedere [Autenticazione basata su password con Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Configurare SSO basato su password**

1. [Configurare l'accesso Single #A0](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) basato su password: in questo articolo vengono fornite informazioni più dettagliate sull'opzione SSO basata su password. Se l'applicazione che si sta aggiungendo richiede una configurazione personalizzata ed è necessario utilizzare SSO basato su password, questo articolo fa per te.
2. [Configurare l'accesso Single #A0 basato](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) su password per le app in modalità on-prem: il proxy dell'applicazione supporta diverse modalità Single Sign-On. L'accesso basato su password è destinato alle applicazioni che utilizzano una combinazione nome utente/password per l'autenticazione. Quando si configura l'accesso basato su password per l'applicazione, gli utenti devono accedere all'applicazione locale una sola volta. Successivamente, Azure Active Directory archivia le informazioni di accesso e le fornisce automaticamente all'applicazione quando gli utenti accedono in remoto.
    - Dovresti aver già pubblicato e testato l'app con proxy di applicazione. In caso contrario, segui i passaggi descritti in Pubblicare le applicazioni usando il proxy dell'applicazione [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) e quindi continuare la configurazione del servizio SSO basato su password per le app in modalità prem.

Per risolvere i problemi relativi all'accesso Single #A0 basato su password, vedere Risolvere i problemi [relativi all'accesso Single #A0 basato su password in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
