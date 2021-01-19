---
title: Risoluzione dei problemi relativi al consenso degli utenti
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897761"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="723c5-102">Risoluzione dei problemi relativi al consenso degli utenti</span><span class="sxs-lookup"><span data-stu-id="723c5-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="723c5-103">È possibile configurare in che modo gli utenti finali acconsentono alle applicazioni tramite il portale di Azure o PowerShell.</span><span class="sxs-lookup"><span data-stu-id="723c5-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="723c5-104">Per ulteriori informazioni, vedere [impostazioni di consenso dell'utente](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .</span><span class="sxs-lookup"><span data-stu-id="723c5-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="723c5-105">Un amministratore può anche utilizzare l' [API di Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) per concedere il consenso alle autorizzazioni delegate per conto di un singolo utente.</span><span class="sxs-lookup"><span data-stu-id="723c5-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="723c5-106">Per ulteriori informazioni, vedere [Get Access per conto di un utente](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="723c5-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="723c5-107">[Errori di consenso dell'utente](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): in questo articolo vengono illustrati gli errori che possono verificarsi durante il processo di consenziente a un'applicazione.</span><span class="sxs-lookup"><span data-stu-id="723c5-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="723c5-108">Se si desidera risolvere i messaggi di errore non consentiti per la risoluzione dei problemi, vedere [scenari di autenticazione di Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="723c5-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>