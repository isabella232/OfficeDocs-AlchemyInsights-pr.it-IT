---
title: Aggiungere un gruppo a un sito di SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758735"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="3014c-102">Creare un sito connesso a un gruppo in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="3014c-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="3014c-103">Durante la creazione o la ricreazione di un sito collegato a un gruppo sono stati riscontrati un paio di problemi comuni.</span><span class="sxs-lookup"><span data-stu-id="3014c-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="3014c-104">Se è stato eliminato un gruppo e il relativo sito connesso e si desidera creare un altro sito con lo stesso URL, è necessario rimuovere definitivamente il sito precedente.</span><span class="sxs-lookup"><span data-stu-id="3014c-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="3014c-105">Scaricare [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="3014c-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="3014c-106">Per altre informazioni sulla Guida introduttiva a PowerShell, vedere [Guida introduttiva a SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="3014c-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="3014c-107">Rimuovere il sito dai siti eliminati utilizzando il cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3014c-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="3014c-108">Se si sta creando un sito collegato a un gruppo e si riceve un avviso un altro gruppo con lo stesso alias esiste già, controllare i gruppi esistenti dall'interfaccia di [amministrazione di Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="3014c-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="3014c-109">Per risolvere il problema, eliminare il gruppo esistente se non è più necessario o creare il sito con un altro alias assegnato.</span><span class="sxs-lookup"><span data-stu-id="3014c-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="3014c-110">Esistono diversi modi per creare e utilizzare i gruppi moderni con SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3014c-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="3014c-111">È possibile connettere i siti esistenti a un gruppo di Office 365.</span><span class="sxs-lookup"><span data-stu-id="3014c-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="3014c-112">Per altre informazioni, vedere [connettere un gruppo di Office 365 utilizzando l'utente di ineterface di SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="3014c-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="3014c-113">Per creare un sito collegato a un gruppo di Office 365, è necessario creare un sito del team.</span><span class="sxs-lookup"><span data-stu-id="3014c-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="3014c-114">Per altre informazioni, vedere [creare un sito del team in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="3014c-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

