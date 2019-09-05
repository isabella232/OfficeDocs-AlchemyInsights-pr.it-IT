---
title: Creare un sito di SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738201"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="c7639-102">Creare un sito di SharePoint</span><span class="sxs-lookup"><span data-stu-id="c7639-102">Create a SharePoint site</span></span>

<span data-ttu-id="c7639-103">Per informazioni sulla creazione di siti di SharePoint, è possibile visualizzare i seguenti elementi:</span><span class="sxs-lookup"><span data-stu-id="c7639-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="c7639-104">[Gestire i siti nella nuova interfaccia di amministrazione di SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): informazioni sulle opzioni di creazione del sito, tra cui la modalità di creazione di un sito classico o di un sito di team che non include un gruppo di Office 365.</span><span class="sxs-lookup"><span data-stu-id="c7639-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="c7639-105">[Creare un sito del team in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): informazioni su come creare un sito del team.</span><span class="sxs-lookup"><span data-stu-id="c7639-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="c7639-106">[Creare un sito di comunicazione in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): informazioni su come creare un sito di comunicazione.</span><span class="sxs-lookup"><span data-stu-id="c7639-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="c7639-107">[Gestire i siti nella nuova](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site)interfaccia di amministrazione di SharePoint: informazioni su come creare un sito classico o un sito del team che non includa un gruppo di Office 365.</span><span class="sxs-lookup"><span data-stu-id="c7639-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="c7639-108">[! Consigli</span><span class="sxs-lookup"><span data-stu-id="c7639-108">[!Tips]</span></span>
> - <span data-ttu-id="c7639-109">Non è possibile creare un sito con lo stesso URL di un sito esistente.</span><span class="sxs-lookup"><span data-stu-id="c7639-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="c7639-110">Se si è eliminato un sito e si desidera riutilizzare l'URL, è possibile che il sito eliminato esista ancora in **siti eliminati**.</span><span class="sxs-lookup"><span data-stu-id="c7639-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="c7639-111">Per gestire i siti eliminati, vedere [eliminare un sito](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="c7639-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="c7639-112">Per rimuovere completamente un sito con PowerShell, vedere l'esempio relativo al cmdlet [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="c7639-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="c7639-113">Alcuni utenti potrebbero non essere in grado di creare un sito.</span><span class="sxs-lookup"><span data-stu-id="c7639-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="c7639-114">Vedere [gestire la creazione di siti in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="c7639-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="c7639-115">È possibile che il sito venga visualizzato bloccato durante la **creazione** di un periodo di tempo superiore a quello previsto.</span><span class="sxs-lookup"><span data-stu-id="c7639-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="c7639-116">Se sono passate più di 24 ore da quando hai visto questo problema, registra un ticket di supporto.</span><span class="sxs-lookup"><span data-stu-id="c7639-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="c7639-117">In molti casi, stiamo già lavorando a una soluzione.</span><span class="sxs-lookup"><span data-stu-id="c7639-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="c7639-118">Per completare una soluzione, è possibile fornirci almeno 24 ore.</span><span class="sxs-lookup"><span data-stu-id="c7639-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="c7639-119">Se è necessario creare un nuovo sito del team che non includa un gruppo di Office 365,</span><span class="sxs-lookup"><span data-stu-id="c7639-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


