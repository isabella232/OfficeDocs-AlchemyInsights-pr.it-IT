---
title: Ripristinare una cartella pubblica eliminata
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809443"
---
# <a name="restore-a-deleted-public-folder"></a>Ripristinare una cartella pubblica eliminata

**Per ripristinare gli elementi eliminati da una cartella pubblica:**

- Vedere Non è possibile recuperare gli elementi eliminati da una cartella pubblica non di posta [elettronica in Outlook 2016.](https://aka.ms/pfrec)
 
**Per ripristinare una cartella pubblica eliminata (di qualsiasi tipo):** 

- Utilizzare il seguente comando exO PowerShell:

    Sintassi:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Esempio: il comando seguente ripristina Subfolder1 e lo posiziona in \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Per [ulteriori informazioni, vedere Restore a deleted public folder.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
