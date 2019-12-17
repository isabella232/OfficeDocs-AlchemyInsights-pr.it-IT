---
title: Problemi relativi alle autorizzazioni durante la migrazione
ms.author: pebaum
author: pebaum
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 95bfbfdf002e457230479a860058c1cf7ab1f8c2
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054418"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="155bc-102">Sincronizzazione dei profili utente e delle foto</span><span class="sxs-lookup"><span data-stu-id="155bc-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="155bc-103">**Sincronizzazione foto profilo** : gli utenti possono notare che la foto del profilo non è in grado di eseguire la sincronizzazione con SharePoint.</span><span class="sxs-lookup"><span data-stu-id="155bc-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="155bc-104">In alternativa, possono aver tentato di aggiornare la foto del profilo e la foto viene visualizzata ancora come vecchia foto.</span><span class="sxs-lookup"><span data-stu-id="155bc-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="155bc-105">Per assicurarsi che la foto del profilo venga visualizzata come previsto, l'utente dovrà avviare una sincronizzazione delle foto.</span><span class="sxs-lookup"><span data-stu-id="155bc-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="155bc-106">Per ulteriori informazioni sul processo di sincronizzazione delle foto, vedere [informazioni sulla sincronizzazione delle immagini dei profili in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="155bc-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="155bc-107">**Sincronizzazione dei profili** : il tempo necessario per completare una sincronizzazione dei profili dipende dal numero di modifiche (lavoro) che il processo di importazione degli annunci deve elaborare.</span><span class="sxs-lookup"><span data-stu-id="155bc-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="155bc-108">Se sono presenti molte modifiche, il processo timer ha molto lavoro da fare e richiederà più tempo affinché le modifiche vengano riflesse nell'applicazione profilo utente.</span><span class="sxs-lookup"><span data-stu-id="155bc-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="155bc-109">Se il processo timer ha un volume minimo di lavoro da eseguire, le modifiche verranno riflesse nell'applicazione profilo utente molto più velocemente.</span><span class="sxs-lookup"><span data-stu-id="155bc-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="155bc-110">Per ulteriori informazioni sul processo di sincronizzazione del profilo, vedere [informazioni sulla sincronizzazione dei profili utente in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="155bc-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="155bc-111">L' **aggiornamento del profilo in Office approfondire** gli utenti può gestire il profilo di Office 365.</span><span class="sxs-lookup"><span data-stu-id="155bc-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="155bc-112">Per ulteriori informazioni, vedere [View and Update your profile in Office approfondire](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="155bc-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

