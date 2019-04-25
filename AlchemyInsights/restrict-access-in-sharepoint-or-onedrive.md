---
title: Limitare l'accesso in SharePoint o OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383875"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Limitare l'accesso in SharePoint o OneDrive

In SharePoint e OneDrive, è possibile limitare l'accesso a elementi quali file, cartelle ed elenchi concedendo l'accesso solo ai gruppi o alle persone a cui si desidera accedere. Per impostazione predefinita, le autorizzazioni in SharePoint vengono ereditate dall'alto nella gerarchia. In questo modo un file eredita le autorizzazioni dalla cartella, che eredita le autorizzazioni dalla raccolta, che eredita le autorizzazioni dal sito.
  
È possibile condividere a un livello superiore, ad esempio la condivisione di un intero sito, e quindi interrompere l'ereditarietà se non si desidera condividere tutti gli elementi del sito. Tuttavia, non è consigliabile perché rende più complesse e confuse le autorizzazioni per il futuro. Ecco cosa si potrebbe fare, invece:
  
- Se, ad esempio, si desidera condividere tutto il contenuto di una cartella ad eccezione di un file in esso, spostare il file in una nuova posizione che non è condivisa.
    
- Se si dispone di due sottocartelle in una cartella e si desidera condividere una sottocartella con i gruppi A e B e consentire l'accesso solo al gruppo a alla seconda sottocartella, condividere la cartella padre con il gruppo A e aggiungere il gruppo B alla prima sottocartella.
    
[Interrompere la condivisione di un file o una cartella](https://go.microsoft.com/fwlink/?linkid=2008861)
  

