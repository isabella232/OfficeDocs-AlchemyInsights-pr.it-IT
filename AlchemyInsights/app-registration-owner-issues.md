---
title: Problemi relativi al proprietario della registrazione dell'app
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123195"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="ede7a-102">Problemi relativi al proprietario della registrazione dell'app</span><span class="sxs-lookup"><span data-stu-id="ede7a-102">App Registration Owner issues</span></span>

<span data-ttu-id="ede7a-103">Di seguito sono riportati i metodi disponibili per aggiungere entità come proprietari per le registrazioni delle app:</span><span class="sxs-lookup"><span data-stu-id="ede7a-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="ede7a-104">Utilizzo del modulo di Azure AD PowerShell -</span><span class="sxs-lookup"><span data-stu-id="ede7a-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="ede7a-105">Riferimento: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="ede7a-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="ede7a-106">Utilizzo dell'interfaccia della riga di comando di Azure - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="ede7a-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="ede7a-107">Riferimento: [proprietario dell'app pubblicitaria az](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="ede7a-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="ede7a-108">Utilizzo di MS Graph -</span><span class="sxs-lookup"><span data-stu-id="ede7a-108">Using MS Graph -</span></span>

    <span data-ttu-id="ede7a-109">Riferimento: [Aggiungere proprietario - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="ede7a-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="ede7a-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span><span class="sxs-lookup"><span data-stu-id="ede7a-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="ede7a-111">**Non è possibile visualizzare l'applicazione nel pannello Registrazioni app anche se si è proprietari di tale applicazione?**</span><span class="sxs-lookup"><span data-stu-id="ede7a-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="ede7a-112">Il proprietario di un'app non è un ruolo amministrativo.</span><span class="sxs-lookup"><span data-stu-id="ede7a-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="ede7a-113">Se [l'impostazione Limita accesso al portale di amministrazione](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) di Azure AD è abilitata, solo l'amministratore potrà visualizzare le applicazioni nel portale di registrazione app.</span><span class="sxs-lookup"><span data-stu-id="ede7a-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="ede7a-114">Per fare in modo che un proprietario possa visualizzare le applicazioni, disabilitare questa impostazione (impostare questa opzione su NO) o assegnare il ruolo di amministratore al proprietario solo per l'applicazione specifica.</span><span class="sxs-lookup"><span data-stu-id="ede7a-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="ede7a-115">A questo scopo, tuttavia, sarà necessaria una licenza di Azure AD Premium P2 e si abiliterà [Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="ede7a-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
