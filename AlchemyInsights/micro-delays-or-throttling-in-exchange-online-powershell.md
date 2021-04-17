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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830037"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="511f1-102">Micro ritardi o limitazione in PowerShell per Exchange Online</span><span class="sxs-lookup"><span data-stu-id="511f1-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="511f1-103">Durante l'esecuzione di script e cmdlet in Exchange Online potrebbero verificarsi ritardi o potrebbero comparire avvisi "Applicato micro ritardo".</span><span class="sxs-lookup"><span data-stu-id="511f1-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="511f1-104">Ecco due suggerimenti a questo proposito:</span><span class="sxs-lookup"><span data-stu-id="511f1-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="511f1-105">Provare a usare il [modulo PowerShell per Exchange Online v2](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), che include CMDlet basati sull'API REST e nettamente più performanti.</span><span class="sxs-lookup"><span data-stu-id="511f1-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="511f1-106">Può essere un'ottima soluzione per molti CMDlet Get che vengono usati di frequente.</span><span class="sxs-lookup"><span data-stu-id="511f1-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="511f1-107">Se è necessario usare CMDlet non ancora coperti dal modulo v2, vedere l'argomento relativo all'[esecuzione di cmdlet di PowerShell per un numero elevato di utenti in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), che illustra come ovviare ai limiti previsti di PowerShell in Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="511f1-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
