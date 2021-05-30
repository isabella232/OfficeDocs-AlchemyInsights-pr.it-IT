---
title: Micro ritardi o limitazione in PowerShell per Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702130"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="ddde7-102">Micro ritardi o limitazione in PowerShell per Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ddde7-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="ddde7-103">Durante l'esecuzione di script e cmdlet in Exchange Online potrebbero verificarsi ritardi o potrebbero comparire avvisi "Applicato micro ritardo".</span><span class="sxs-lookup"><span data-stu-id="ddde7-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="ddde7-104">Seguono alcuni suggerimenti su come risolvere questo problema:</span><span class="sxs-lookup"><span data-stu-id="ddde7-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="ddde7-105">Eseguire la diagnostica per rivedere i criteri di limitazione di PowerShell del tenant.</span><span class="sxs-lookup"><span data-stu-id="ddde7-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="ddde7-106">Nella maggior parte dei casi, questa soluzione risolverà il problema.</span><span class="sxs-lookup"><span data-stu-id="ddde7-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="ddde7-107">Se il problema non dovesse essersi risolto, provare a usare il [modulo PowerShell per Exchange Online v2](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), che include CMDlet basati sull'API REST e nettamente più performanti.</span><span class="sxs-lookup"><span data-stu-id="ddde7-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="ddde7-108">Può essere un'ottima soluzione per molti CMDlet Get che vengono usati di frequente.</span><span class="sxs-lookup"><span data-stu-id="ddde7-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="ddde7-109">Se è necessario usare CMDlet non coperti dal modulo v2, vedere l'argomento relativo all'[esecuzione di cmdlet di PowerShell per un numero elevato di utenti in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), che illustra come ovviare ai limiti di PowerShell in Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ddde7-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
