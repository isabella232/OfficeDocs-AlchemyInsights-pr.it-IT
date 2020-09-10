---
title: Controllare l'accesso alle cartelle pubbliche con Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: b04e09f5110266d59db82e25cfda1835779fd4b7
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406581"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="62f64-102">Controllare l'accesso alle cartelle pubbliche con Outlook</span><span class="sxs-lookup"><span data-stu-id="62f64-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="62f64-103">Per controllare quali utenti possono accedere alle cartelle pubbliche con Outlook:</span><span class="sxs-lookup"><span data-stu-id="62f64-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="62f64-104">Usare `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="62f64-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="62f64-105">$true: consente agli utenti di accedere alle cartelle pubbliche in Outlook</span><span class="sxs-lookup"><span data-stu-id="62f64-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="62f64-106">$false: consente agli utenti di accedere alle cartelle pubbliche in Outlook. </span><span class="sxs-lookup"><span data-stu-id="62f64-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="62f64-107">Questo è il valore predefinito.</span><span class="sxs-lookup"><span data-stu-id="62f64-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="62f64-108">Nota: questa procedura può solo controllare le connessioni con i client desktop di Outlook per Windows.</span><span class="sxs-lookup"><span data-stu-id="62f64-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="62f64-109">Gli utenti possono continuare ad accedere alle cartelle pubbliche con OWA o Outlook per Mac.</span><span class="sxs-lookup"><span data-stu-id="62f64-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="62f64-110">Per altre informazioni, vedere [Connessioni controllate per le cartelle pubbliche di Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="62f64-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
