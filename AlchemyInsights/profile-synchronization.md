---
title: Sincronizzazione dei profili
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296313"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="93eb0-102">Quando le modifiche profilo sincronizzare per l'applicazione profili utente di SharePoint?</span><span class="sxs-lookup"><span data-stu-id="93eb0-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="93eb0-103">SharePoint Online, il processo timer di importazione Active Directory (importazione Active Directory) viene utilizzato per importare gli utenti e gruppi in applicazione profili utente.</span><span class="sxs-lookup"><span data-stu-id="93eb0-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="93eb0-p101">Importazione Active Directory esegue la sincronizzazione delle modifiche dall'archivio Directory SharePoint Online per l'applicazione profili utente. Queste modifiche vengono elaborate in batch.</span><span class="sxs-lookup"><span data-stu-id="93eb0-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="93eb0-106">Il processo timer viene eseguito fino a quando non vengono sincronizzate le modifiche.</span><span class="sxs-lookup"><span data-stu-id="93eb0-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="93eb0-p102">Il tempo di esecuzione del processo dipende dal numero di modifiche apportate al processo. Un numero elevato di modifiche richiede più tempo. Service Level Agreement (SLA) indica che una modifica apportata a un utente in SharePoint Online Directory verrà riflettersi nell'applicazione profili utente in 24 ore.</span><span class="sxs-lookup"><span data-stu-id="93eb0-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="93eb0-110">Ulteriori informazioni sulla sincronizzazione dei profili utente in SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="93eb0-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

