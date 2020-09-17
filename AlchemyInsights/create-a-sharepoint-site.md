---
title: Creare un sito di SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806943"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="ce2d4-102">Creare un sito di SharePoint</span><span class="sxs-lookup"><span data-stu-id="ce2d4-102">Create a SharePoint site</span></span>

<span data-ttu-id="ce2d4-103">Creare o gestire siti da [siti attivi](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) nell'interfaccia di amministrazione di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ce2d4-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="ce2d4-104">Per altre informazioni, vedere [gestire i siti nella nuova interfaccia di amministrazione di SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="ce2d4-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="ce2d4-105">Consigli</span><span class="sxs-lookup"><span data-stu-id="ce2d4-105">Tips:</span></span>

- <span data-ttu-id="ce2d4-106">**Non è possibile** creare un sito con lo stesso URL di un sito esistente.</span><span class="sxs-lookup"><span data-stu-id="ce2d4-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="ce2d4-107">Se si è eliminato un sito e si desidera riutilizzare l'URL, è possibile che il sito eliminato esista ancora in [siti eliminati](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="ce2d4-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="ce2d4-108">Il sito dovrà essere eliminato definitivamente per riutilizzare l'URL.</span><span class="sxs-lookup"><span data-stu-id="ce2d4-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="ce2d4-109">Per rimuovere completamente un sito con PowerShell, vedere l'esempio relativo al cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="ce2d4-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="ce2d4-110">Alcuni utenti potrebbero non essere in grado di creare un sito.</span><span class="sxs-lookup"><span data-stu-id="ce2d4-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="ce2d4-111">[Vedere gestire la creazione di siti in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="ce2d4-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="ce2d4-112">È possibile che il sito venga visualizzato bloccato durante la **creazione** di un periodo di tempo superiore a quello previsto.</span><span class="sxs-lookup"><span data-stu-id="ce2d4-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="ce2d4-113">Se sono passate più di 24 ore da quando hai visto questo problema, registra un ticket di supporto.</span><span class="sxs-lookup"><span data-stu-id="ce2d4-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="ce2d4-114">In molti casi, stiamo già lavorando a una soluzione.</span><span class="sxs-lookup"><span data-stu-id="ce2d4-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="ce2d4-115">Per completare una soluzione, è possibile fornirci almeno 24 ore.</span><span class="sxs-lookup"><span data-stu-id="ce2d4-115">Please give us at least 24 hours to complete a solution.</span></span>
