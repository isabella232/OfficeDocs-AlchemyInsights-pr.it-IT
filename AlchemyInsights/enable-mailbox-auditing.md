---
title: Abilitare il controllo delle cassette postali
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703575"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="405d8-102">Abilitare il controllo delle cassette postali</span><span class="sxs-lookup"><span data-stu-id="405d8-102">Enable mailbox auditing</span></span>

<span data-ttu-id="405d8-103">Per abilitare il controllo delle cassette postali per un singolo utente o per un'intera organizzazione, è necessario eseguire i cmdlet seguenti da Remote Power Shell:</span><span class="sxs-lookup"><span data-stu-id="405d8-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="405d8-104">**Singolo utente**</span><span class="sxs-lookup"><span data-stu-id="405d8-104">**Single User**</span></span>
  
<span data-ttu-id="405d8-105">Set-Mailbox-Identity "Jane Dow"-AuditEnabled consente $true</span><span class="sxs-lookup"><span data-stu-id="405d8-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="405d8-106">**Organizzazione**</span><span class="sxs-lookup"><span data-stu-id="405d8-106">**Organization**</span></span>
  
<span data-ttu-id="405d8-107">Get-Mailbox-ResultSize Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled consente $true</span><span class="sxs-lookup"><span data-stu-id="405d8-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="405d8-108">Altre informazioni</span><span class="sxs-lookup"><span data-stu-id="405d8-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

