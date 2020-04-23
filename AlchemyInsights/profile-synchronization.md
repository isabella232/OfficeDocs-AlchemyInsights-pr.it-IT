---
title: Sincronizzazione dei profili
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768117"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="80d10-102">Quando il mio profilo cambia la sincronizzazione con l'applicazione profilo utente di SharePoint?</span><span class="sxs-lookup"><span data-stu-id="80d10-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="80d10-103">SharePoint Online utilizza il processo timer di importazione di Active Directory (AD Import) per importare gli utenti e i gruppi nell'applicazione profili utente.</span><span class="sxs-lookup"><span data-stu-id="80d10-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="80d10-104">Importazione di Active Directory consente di sincronizzare le modifiche apportate all'applicazione profilo utente dall'archivio di elenchi di SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="80d10-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="80d10-105">Queste modifiche vengono elaborate in batch.</span><span class="sxs-lookup"><span data-stu-id="80d10-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="80d10-106">Il processo timer viene eseguito fino a quando le modifiche non vengono sincronizzate.</span><span class="sxs-lookup"><span data-stu-id="80d10-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="80d10-107">Il tempo necessario per l'esecuzione del processo dipende dal numero di modifiche apportate.</span><span class="sxs-lookup"><span data-stu-id="80d10-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="80d10-108">Un numero elevato di modifiche richiede più tempo.</span><span class="sxs-lookup"><span data-stu-id="80d10-108">A large number of changes takes longer.</span></span> <span data-ttu-id="80d10-109">Il contratto di servizio stabilisce che una modifica apportata a un utente nella directory di SharePoint Online verrà riflessa nell'applicazione profilo utente in 24 ore.</span><span class="sxs-lookup"><span data-stu-id="80d10-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="80d10-110">Altre informazioni sulla sincronizzazione dei profili utente in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="80d10-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

