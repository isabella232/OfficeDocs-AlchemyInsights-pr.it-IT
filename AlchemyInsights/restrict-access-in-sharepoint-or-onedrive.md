---
title: Limitare l'accesso in SharePoint o OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720686"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Limitare l'accesso in SharePoint o OneDrive

In SharePoint e OneDrive, è possibile limitare l'accesso a elementi quali file, cartelle ed elenchi concedendo l'accesso solo ai gruppi o alle persone a cui si desidera accedere. Per impostazione predefinita, le autorizzazioni in SharePoint vengono ereditate dall'alto nella gerarchia. In questo modo un file eredita le autorizzazioni dalla cartella, che eredita le autorizzazioni dalla raccolta, che eredita le autorizzazioni dal sito.
  
È possibile condividere a un livello superiore, ad esempio la condivisione di un intero sito, e quindi interrompere l'ereditarietà se non si desidera condividere tutti gli elementi del sito. Tuttavia, non è consigliabile perché rende più complesse e confuse le autorizzazioni per il futuro. Ecco cosa si potrebbe fare, invece:
  
- Se, ad esempio, si desidera condividere tutto il contenuto di una cartella ad eccezione di un file in esso, spostare il file in una nuova posizione che non è condivisa.
    
- Se si dispone di due sottocartelle in una cartella e si desidera condividere una sottocartella con i gruppi A e B e consentire l'accesso solo al gruppo a alla seconda sottocartella, condividere la cartella padre con il gruppo A e aggiungere il gruppo B alla prima sottocartella.
    
[Interrompere la condivisione di un file o una cartella ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

