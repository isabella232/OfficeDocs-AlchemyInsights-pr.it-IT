---
title: Sincronizzazione dei profili
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29920092"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando le modifiche profilo sincronizzare per l'applicazione profili utente di SharePoint?

SharePoint Online, il processo timer di importazione Active Directory (importazione Active Directory) viene utilizzato per importare gli utenti e gruppi in applicazione profili utente. 
  
1. Importazione Active Directory esegue la sincronizzazione delle modifiche dall'archivio Directory SharePoint Online per l'applicazione profili utente. Queste modifiche vengono elaborate in batch.
    
2. Il processo timer viene eseguito fino a quando non vengono sincronizzate le modifiche.
    
> [!NOTE]
> Il tempo di esecuzione del processo dipende dal numero di modifiche apportate al processo. Un numero elevato di modifiche richiede più tempo. Service Level Agreement (SLA) indica che una modifica apportata a un utente in SharePoint Online Directory verrà riflettersi nell'applicazione profili utente in 24 ore. 
  
[Ulteriori informazioni sulla sincronizzazione dei profili utente in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

