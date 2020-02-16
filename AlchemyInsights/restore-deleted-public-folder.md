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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="7510f-102">Ripristinare una cartella pubblica eliminata</span><span class="sxs-lookup"><span data-stu-id="7510f-102">Restore a deleted public folder</span></span>

<span data-ttu-id="7510f-103">**Per ripristinare gli elementi eliminati da una cartella pubblica**:</span><span class="sxs-lookup"><span data-stu-id="7510f-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="7510f-104">Vedere non [è possibile recuperare gli elementi eliminati da una cartella pubblica non di posta in Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="7510f-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="7510f-105">**Per ripristinare una cartella pubblica eliminata (di qualsiasi tipo)**:</span><span class="sxs-lookup"><span data-stu-id="7510f-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="7510f-106">Utilizzare il seguente comando di EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7510f-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="7510f-107">Sintassi:</span><span class="sxs-lookup"><span data-stu-id="7510f-107">Syntax:</span></span>

    ><span data-ttu-id="7510f-108">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Name-eq "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. Identity- \<path percorso in cui verrà ripristinata la cartella></span><span class="sxs-lookup"><span data-stu-id="7510f-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="7510f-109">Esempio: il comando seguente ripristinerà Sottocartella1 e lo inserirà in \Parent1:</span><span class="sxs-lookup"><span data-stu-id="7510f-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="7510f-110">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Name-eq "Sottocartella1"}; Set-PublicFolder $pf. Identity-Path \Parent1</span><span class="sxs-lookup"><span data-stu-id="7510f-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="7510f-111">Per ulteriori informazioni, vedere [ripristinare una cartella pubblica eliminata](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="7510f-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
