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
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320713"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Quando vengono sincronizzate le modifiche al profilo SharePoint'applicazione profilo utente?

SharePoint Online usa il processo timer Importazione di Active Directory (IMPORTAZIONE AD) per importare utenti e gruppi nell'applicazione profili utente. 
  
1. Importazione AD sincronizza le modifiche dall'SharePoint directory online all'applicazione profili utente. Queste modifiche vengono elaborate in batch.
    
2. Il processo timer viene eseguito fino alla sincronizzazione delle modifiche.
    
**Nota:** il tempo necessario per l'esecuzione del processo dipende dal numero di modifiche da elaborare. Un numero elevato di modifiche richiede più tempo. Il Contratto di servizio (SLA) indica che una modifica apportata a un utente nella directory di SharePoint Online verrà riflessa nell'applicazione profili utente in 24 ore. 
  
[Altre info sulla sincronizzazione dei profili utente in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

