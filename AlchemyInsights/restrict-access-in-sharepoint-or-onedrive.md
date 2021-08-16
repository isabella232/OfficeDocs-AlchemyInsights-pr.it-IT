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
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075044"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Limitare l'accesso in SharePoint o OneDrive

In SharePoint e OneDrive, è possibile limitare l'accesso a elementi come file, cartelle ed elenchi concedendo l'accesso solo a gruppi o utenti a cui si desidera accedere. Per impostazione predefinita, le autorizzazioni SharePoint vengono ereditate dall'alto verso l'alto nella gerarchia. Un file eredita quindi le autorizzazioni dalla cartella, che eredita le autorizzazioni dalla raccolta, che eredita le autorizzazioni dal sito.
  
È possibile condividere a un livello superiore, ad esempio condividendo un intero sito, e quindi interrompere l'ereditarietà se non si desidera condividere tutti gli elementi nel sito. Tuttavia, non è consigliabile farlo perché in futuro la gestione delle autorizzazioni sarà più complessa e confusa. Ecco cosa puoi fare invece:
  
- Se, ad esempio, si desidera condividere tutto il contenuto di una cartella ad eccezione di un file in essa contenuto, spostare il file in un nuovo percorso non condiviso.
    
- Se si dispone di due sottocartelle in una cartella e si desidera condividere una sottocartella con i gruppi A e B e consentire solo al gruppo A l'accesso alla seconda sottocartella, condividere la cartella padre con il gruppo A e aggiungere il gruppo B alla prima sottocartella.
    
[Interrompere la condivisione di un file o di una cartella ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

