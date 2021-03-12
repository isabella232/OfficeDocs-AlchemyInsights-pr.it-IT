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
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="a7e11-102">Risolvere i problemi relativi all'accesso Single #A0 (SSO) basato su password</span><span class="sxs-lookup"><span data-stu-id="a7e11-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="a7e11-103">Per informazioni sui concetti fondamentali di SSO basato su password, vedere [Autenticazione basata su password con Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="a7e11-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="a7e11-104">**Configurare SSO basato su password**</span><span class="sxs-lookup"><span data-stu-id="a7e11-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="a7e11-105">[Configurare l'accesso Single #A0](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) basato su password: in questo articolo vengono fornite informazioni più dettagliate sull'opzione SSO basata su password.</span><span class="sxs-lookup"><span data-stu-id="a7e11-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="a7e11-106">Se l'applicazione che si sta aggiungendo richiede una configurazione personalizzata ed è necessario utilizzare SSO basato su password, questo articolo fa per te.</span><span class="sxs-lookup"><span data-stu-id="a7e11-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="a7e11-107">[Configurare l'accesso Single #A0 basato](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) su password per le app in modalità on-prem: il proxy dell'applicazione supporta diverse modalità Single Sign-On.</span><span class="sxs-lookup"><span data-stu-id="a7e11-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="a7e11-108">L'accesso basato su password è destinato alle applicazioni che utilizzano una combinazione nome utente/password per l'autenticazione.</span><span class="sxs-lookup"><span data-stu-id="a7e11-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="a7e11-109">Quando si configura l'accesso basato su password per l'applicazione, gli utenti devono accedere all'applicazione locale una sola volta.</span><span class="sxs-lookup"><span data-stu-id="a7e11-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="a7e11-110">Successivamente, Azure Active Directory archivia le informazioni di accesso e le fornisce automaticamente all'applicazione quando gli utenti accedono in remoto.</span><span class="sxs-lookup"><span data-stu-id="a7e11-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="a7e11-111">Dovresti aver già pubblicato e testato l'app con proxy di applicazione.</span><span class="sxs-lookup"><span data-stu-id="a7e11-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="a7e11-112">In caso contrario, segui i passaggi descritti in Pubblicare le applicazioni usando il proxy dell'applicazione [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) e quindi continuare la configurazione del servizio SSO basato su password per le app in modalità prem.</span><span class="sxs-lookup"><span data-stu-id="a7e11-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="a7e11-113">Per risolvere i problemi relativi all'accesso Single #A0 basato su password, vedere Risolvere i problemi [relativi all'accesso Single #A0 basato su password in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="a7e11-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
