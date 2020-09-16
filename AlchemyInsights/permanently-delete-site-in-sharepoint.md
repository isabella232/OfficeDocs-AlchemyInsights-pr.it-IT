---
title: Eliminare definitivamente un sito in SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: bde31f9b197118467ed96d665a9c8edf6b789965
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771725"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="9f9d4-102">Eliminare definitivamente un sito in SharePoint</span><span class="sxs-lookup"><span data-stu-id="9f9d4-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="9f9d4-103">Per riutilizzare un URL di un sito eliminato (per ricreare un sito) oppure per eliminare definitivamente un sito perché non è più in uso, è possibile usare **Elimina definitivamente** dalla nuova interfaccia di amministrazione di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9f9d4-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="9f9d4-104">Passare alla [pagina Siti eliminati della nuova interfaccia di amministrazione di SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) e accedere con un account dotato di autorizzazioni di amministratore per l'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="9f9d4-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="9f9d4-105">Nella colonna sinistra selezionare un sito.</span><span class="sxs-lookup"><span data-stu-id="9f9d4-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="9f9d4-106">Fare clic su **Elimina definitivamente**.</span><span class="sxs-lookup"><span data-stu-id="9f9d4-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="9f9d4-107">**Nota**: i siti connessi a un gruppo non possono essere eliminati definitivamente dalla nuova interfaccia di amministrazione di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9f9d4-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="9f9d4-108">È necessario usare il cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="9f9d4-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="9f9d4-109">Per ulteriori informazioni, vedere [Eliminare definitivamente un sito](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="9f9d4-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
