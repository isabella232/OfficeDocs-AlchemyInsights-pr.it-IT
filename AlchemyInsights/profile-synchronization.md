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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando il mio profilo cambia la sincronizzazione con l'applicazione profilo utente di SharePoint?

SharePoint Online utilizza il processo timer di importazione di Active Directory (AD Import) per importare gli utenti e i gruppi nell'applicazione profili utente. 
  
1. Importazione di Active Directory consente di sincronizzare le modifiche apportate all'applicazione profilo utente dall'archivio di elenchi di SharePoint Online. Queste modifiche vengono elaborate in batch.
    
2. Il processo timer viene eseguito fino a quando le modifiche non vengono sincronizzate.
    
> [!NOTE]
> Il tempo necessario per l'esecuzione del processo dipende dal numero di modifiche apportate. Un numero elevato di modifiche richiede più tempo. Il contratto di servizio stabilisce che una modifica apportata a un utente nella directory di SharePoint Online verrà riflessa nell'applicazione profilo utente in 24 ore. 
  
[Altre informazioni sulla sincronizzazione dei profili utente in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

