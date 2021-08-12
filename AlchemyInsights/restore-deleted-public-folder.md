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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943379"
---
# <a name="restore-a-deleted-public-folder"></a>Ripristinare una cartella pubblica eliminata

**Per ripristinare gli elementi eliminati da una cartella pubblica:**

- Vedere [Non è possibile recuperare gli elementi eliminati da una cartella](https://aka.ms/pfrec)pubblica non di posta elettronica in Outlook 2016 .
 
**Per ripristinare una cartella pubblica eliminata (di qualsiasi tipo):** 

- Utilizzare il seguente comando exO PowerShell:

    Sintassi:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Esempio: il comando seguente ripristina Subfolder1 e lo posiziona in \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Per [ulteriori informazioni, vedere Restore a deleted public folder.](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)
