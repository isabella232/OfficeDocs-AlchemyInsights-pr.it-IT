---
title: Controllare l'accesso alle cartelle pubbliche con Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680486"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="e43a6-102">Controllare l'accesso alle cartelle pubbliche con Outlook</span><span class="sxs-lookup"><span data-stu-id="e43a6-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="e43a6-103">Per controllare quali utenti possono accedere alle cartelle pubbliche con Outlook:</span><span class="sxs-lookup"><span data-stu-id="e43a6-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="e43a6-104">Usare `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="e43a6-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="e43a6-105">$true: consente agli utenti di accedere alle cartelle pubbliche in Outlook</span><span class="sxs-lookup"><span data-stu-id="e43a6-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="e43a6-106">$false: consente agli utenti di accedere alle cartelle pubbliche in Outlook. </span><span class="sxs-lookup"><span data-stu-id="e43a6-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="e43a6-107">Questo è il valore predefinito.</span><span class="sxs-lookup"><span data-stu-id="e43a6-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="e43a6-108">Nota: questa procedura può solo controllare le connessioni con i client desktop di Outlook per Windows.</span><span class="sxs-lookup"><span data-stu-id="e43a6-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="e43a6-109">Gli utenti possono continuare ad accedere alle cartelle pubbliche con OWA o Outlook per Mac.</span><span class="sxs-lookup"><span data-stu-id="e43a6-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="e43a6-110">Per altre informazioni, vedere [Connessioni controllate per le cartelle pubbliche di Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="e43a6-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
