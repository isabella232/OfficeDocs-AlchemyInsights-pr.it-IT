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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="cb4be-102">Ripristinare una cartella pubblica eliminata</span><span class="sxs-lookup"><span data-stu-id="cb4be-102">Restore a deleted public folder</span></span>

<span data-ttu-id="cb4be-103">**Per ripristinare gli elementi eliminati da una cartella pubblica**:</span><span class="sxs-lookup"><span data-stu-id="cb4be-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="cb4be-104">Vedere non [è possibile recuperare gli elementi eliminati da una cartella pubblica non di posta in Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="cb4be-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="cb4be-105">**Per ripristinare una cartella pubblica eliminata (di qualsiasi tipo)**:</span><span class="sxs-lookup"><span data-stu-id="cb4be-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="cb4be-106">Utilizzare il seguente comando di EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="cb4be-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="cb4be-107">Sintassi:</span><span class="sxs-lookup"><span data-stu-id="cb4be-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="cb4be-108">Esempio: il comando seguente ripristinerà Sottocartella1 e lo inserirà in \Parent1:</span><span class="sxs-lookup"><span data-stu-id="cb4be-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="cb4be-109">Per ulteriori informazioni, vedere [ripristinare una cartella pubblica eliminata](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="cb4be-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
