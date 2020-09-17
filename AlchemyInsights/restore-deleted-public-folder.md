---
title: Ripristinare una cartella pubblica eliminata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774535"
---
# <a name="restore-a-deleted-public-folder"></a>Ripristinare una cartella pubblica eliminata

**Per ripristinare gli elementi eliminati da una cartella pubblica**:

- Vedere non [è possibile recuperare gli elementi eliminati da una cartella pubblica non di posta in Outlook 2016](https://aka.ms/pfrec).
 
**Per ripristinare una cartella pubblica eliminata (di qualsiasi tipo)**: 

- Utilizzare il seguente comando di EXO PowerShell:

    Sintassi:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Esempio: il comando seguente ripristinerà Sottocartella1 e lo inserirà in \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Per ulteriori informazioni, vedere [ripristinare una cartella pubblica eliminata](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
