---
title: Sincronizzazione dei profili
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801773"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando il mio profilo cambia la sincronizzazione con l'applicazione profilo utente di SharePoint?

SharePoint Online utilizza il processo timer di importazione di Active Directory (AD Import) per importare gli utenti e i gruppi nell'applicazione profili utente. 
  
1. Importazione di Active Directory consente di sincronizzare le modifiche apportate all'applicazione profilo utente dall'archivio di elenchi di SharePoint Online. Queste modifiche vengono elaborate in batch.
    
2. Il processo timer viene eseguito fino a quando le modifiche non vengono sincronizzate.
    
> [!NOTE]
> Il tempo necessario per l'esecuzione del processo dipende dal numero di modifiche apportate. Un numero elevato di modifiche richiede più tempo. Il contratto di servizio stabilisce che una modifica apportata a un utente nella directory di SharePoint Online verrà riflessa nell'applicazione profilo utente in 24 ore. 
  
[Altre informazioni sulla sincronizzazione dei profili utente in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

