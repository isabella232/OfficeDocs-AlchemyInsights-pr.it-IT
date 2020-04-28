---
title: Aggiungere un gruppo a un sito di SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912970"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="cce40-102">Problemi durante la creazione di un sito collegato a un gruppo in SharePoint</span><span class="sxs-lookup"><span data-stu-id="cce40-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="cce40-103">Alcuni problemi comuni riscontrati durante la creazione o la ricreazione di un sito collegato a un gruppo.</span><span class="sxs-lookup"><span data-stu-id="cce40-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="cce40-104">Se è stato eliminato un gruppo e il relativo sito connesso e si desidera creare un altro sito con lo stesso URL, è necessario rimuovere definitivamente il sito precedente.</span><span class="sxs-lookup"><span data-stu-id="cce40-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="cce40-105">Scaricare [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="cce40-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="cce40-106">Per altre informazioni sulla Guida introduttiva a PowerShell, vedere [Guida introduttiva a SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="cce40-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="cce40-107">Rimuovere il sito dai siti eliminati utilizzando il cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cce40-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="cce40-108">PowerShell è necessario per eliminare definitivamente i siti del gruppo.</span><span class="sxs-lookup"><span data-stu-id="cce40-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="cce40-109">Se si sta creando un sito collegato a un gruppo e viene visualizzato un messaggio di avviso: **esiste già un altro gruppo con lo stesso alias**, controllare i gruppi esistenti dall'interfaccia di [amministrazione di Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="cce40-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="cce40-110">Per risolvere il problema, eliminare il gruppo esistente se non è più necessario o creare il sito con un altro alias assegnato.</span><span class="sxs-lookup"><span data-stu-id="cce40-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="cce40-111">Esistono diversi modi per creare e utilizzare i gruppi moderni con SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cce40-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="cce40-112">È possibile connettere i siti esistenti a un gruppo di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cce40-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="cce40-113">Per altre informazioni, vedere [connettere un gruppo di Microsoft 365 utilizzando l'interfaccia utente di SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="cce40-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="cce40-114">Per creare un sito collegato a un gruppo di Microsoft 365, è necessario creare un [sito del team](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="cce40-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
