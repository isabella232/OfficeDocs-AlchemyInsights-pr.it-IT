---
title: Abilitare il controllo delle cassette postali
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736257"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="a6a06-102">Abilitare il controllo delle cassette postali</span><span class="sxs-lookup"><span data-stu-id="a6a06-102">Enable mailbox auditing</span></span>

<span data-ttu-id="a6a06-103">Per abilitare il controllo delle cassette postali per un singolo utente o per un'intera organizzazione, è necessario eseguire i cmdlet seguenti da Remote Power Shell:</span><span class="sxs-lookup"><span data-stu-id="a6a06-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="a6a06-104">**Singolo utente**</span><span class="sxs-lookup"><span data-stu-id="a6a06-104">**Single User**</span></span>
  
<span data-ttu-id="a6a06-105">Set-Mailbox-Identity "Jane Dow"-AuditEnabled consente $true</span><span class="sxs-lookup"><span data-stu-id="a6a06-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="a6a06-106">**Organizzazione**</span><span class="sxs-lookup"><span data-stu-id="a6a06-106">**Organization**</span></span>
  
<span data-ttu-id="a6a06-107">Get-Mailbox-ResultSize Unlimited-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled consente $true</span><span class="sxs-lookup"><span data-stu-id="a6a06-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="a6a06-108">Altre informazioni</span><span class="sxs-lookup"><span data-stu-id="a6a06-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

