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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554337"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando il mio profilo cambia la sincronizzazione con l'applicazione profilo utente di SharePoint?

SharePoint Online utilizza il processo timer di importazione di Active Directory (AD Import) per importare gli utenti e i gruppi nell'applicazione profili utente. 
  
1. Importazione di Active Directory consente di sincronizzare le modifiche apportate all'applicazione profilo utente dall'archivio di elenchi di SharePoint Online. Queste modifiche vengono elaborate in batch.
    
2. Il processo timer viene eseguito fino a quando le modifiche non vengono sincronizzate.
    
> [!NOTE]
> Il tempo necessario per l'esecuzione del processo dipende dal numero di modifiche apportate. Un numero elevato di modifiche richiede più tempo. Il contratto di servizio stabilisce che una modifica apportata a un utente nella directory di SharePoint Online verrà riflessa nell'applicazione profilo utente in 24 ore. 
  
[Altre informazioni sulla sincronizzazione dei profili utente in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

