---
title: Ripristinare una cartella pubblica eliminata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063682"
---
# <a name="restore-a-deleted-public-folder"></a>Ripristinare una cartella pubblica eliminata

**Per ripristinare gli elementi eliminati da una cartella pubblica**:

- Vedere non [è possibile recuperare gli elementi eliminati da una cartella pubblica non di posta in Outlook 2016](https://aka.ms/pfrec).
 
**Per ripristinare una cartella pubblica eliminata (di qualsiasi tipo)**: 

- Utilizzare il seguente comando di EXO PowerShell:

    Sintassi:

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Name-eq "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. Identity- \<path percorso in cui verrà ripristinata la cartella>

    Esempio: il comando seguente ripristinerà Sottocartella1 e lo inserirà in \Parent1:

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Name-eq "Sottocartella1"}; Set-PublicFolder $pf. Identity-Path \Parent1

Per ulteriori informazioni, vedere [ripristinare una cartella pubblica eliminata](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
