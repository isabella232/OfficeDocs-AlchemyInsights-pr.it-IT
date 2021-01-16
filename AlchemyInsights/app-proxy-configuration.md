---
title: Configurazione del proxy dell'applicazione
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876559"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="d6868-102">Configurazione del proxy dell'applicazione</span><span class="sxs-lookup"><span data-stu-id="d6868-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="d6868-103">Per informazioni su come configurare un'applicazione proxy di applicazione all'interno di Azure ad per esporre le applicazioni locali al cloud, vedere [How to Configure an application proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)Application.</span><span class="sxs-lookup"><span data-stu-id="d6868-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="d6868-104">Single Sign-on (SSO) consente agli utenti di accedere a un'applicazione senza eseguire l'autenticazione più volte.</span><span class="sxs-lookup"><span data-stu-id="d6868-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="d6868-105">Consente di eseguire l'autenticazione singola nel cloud, in Azure Active Directory e consente al servizio o al connettore di rappresentare l'utente per completare eventuali ulteriori problemi di autenticazione dall'applicazione.</span><span class="sxs-lookup"><span data-stu-id="d6868-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="d6868-106">Per ulteriori informazioni, vedere [come configurare il servizio Single Sign-on in un'applicazione proxy di applicazione](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="d6868-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="d6868-107">Utilizzare [questo articolo](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) per risolvere i problemi comuni che la gente affronta quando si crea una nuova applicazione proxy di applicazione.</span><span class="sxs-lookup"><span data-stu-id="d6868-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="d6868-108">Se si verifica un problema durante l'impostazione dell'autenticazione back-end nell'applicazione, potrebbe essere necessario risolvere i [problemi relativi alla delega vincolata Kerberos per il proxy dell'applicazione](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) o seguire le indicazioni sulla [configurazione di un'applicazione con PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) per risolvere il problema.</span><span class="sxs-lookup"><span data-stu-id="d6868-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
