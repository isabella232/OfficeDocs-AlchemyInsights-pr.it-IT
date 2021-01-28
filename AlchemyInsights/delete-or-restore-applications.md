---
title: Eliminare o ripristinare le applicazioni
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013958"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="07cfa-102">Eliminare o ripristinare le applicazioni</span><span class="sxs-lookup"><span data-stu-id="07cfa-102">Delete or restore applications</span></span>

<span data-ttu-id="07cfa-103">**Per eliminare un'applicazione dal tenant di Azure ad**:</span><span class="sxs-lookup"><span data-stu-id="07cfa-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="07cfa-104">Nel **portale di Azure ad**, selezionare **applicazioni Enterprise**.</span><span class="sxs-lookup"><span data-stu-id="07cfa-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="07cfa-105">Quindi individuare e selezionare l'applicazione che si desidera eliminare.</span><span class="sxs-lookup"><span data-stu-id="07cfa-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="07cfa-106">Nella sezione **Gestisci** del riquadro sinistro selezionare **Proprietà**.</span><span class="sxs-lookup"><span data-stu-id="07cfa-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="07cfa-107">Selezionare **Elimina**, quindi fare clic su **Sì** per confermare che si desidera eliminare l'app dal tenant di Azure ad.</span><span class="sxs-lookup"><span data-stu-id="07cfa-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="07cfa-108">Per ulteriori informazioni su come eliminare un'app, vedere [Guida introduttiva: eliminare un'applicazione dal tenant di Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="07cfa-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="07cfa-109">In PowerShell, il cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) rimuove le configurazioni del proxy di applicazione da un'applicazione specifica in Azure Active Directory ed è in grado di eliminare completamente l'applicazione, se specificata.</span><span class="sxs-lookup"><span data-stu-id="07cfa-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="07cfa-110">È possibile **ripristinare un'applicazione eliminata** tramite PowerShell.</span><span class="sxs-lookup"><span data-stu-id="07cfa-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="07cfa-111">Dopo che l'applicazione che si desidera ripristinare è stata identificata, è possibile ripristinarla utilizzando [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="07cfa-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
