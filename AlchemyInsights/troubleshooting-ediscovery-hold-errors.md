---
title: Risoluzione dei problemi per gli errori nei blocchi ediscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/20/2021
ms.locfileid: "52583755"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="b06fc-102">Risoluzione dei problemi per gli errori nei blocchi ediscovery</span><span class="sxs-lookup"><span data-stu-id="b06fc-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="b06fc-103">Si sono verificati problemi con i blocchi eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="b06fc-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="b06fc-104">Di seguito alcune procedure consigliate da tenere in considerazione: </span><span class="sxs-lookup"><span data-stu-id="b06fc-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="b06fc-105">Controlla lo stato di distribuzione del blocco.</span><span class="sxs-lookup"><span data-stu-id="b06fc-105">Check the hold distribution status.</span></span>  <span data-ttu-id="b06fc-106">Se lo stato è **On (in Sospeso)** o **Off (in Sospeso)**, attendere la completa distribuzione del blocco.</span><span class="sxs-lookup"><span data-stu-id="b06fc-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="b06fc-107">Accorpa gli aggiornamenti del blocco eDiscovery in una singola richiesta invece di aggiornare il criterio ripetutamente per ogni transazione.</span><span class="sxs-lookup"><span data-stu-id="b06fc-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="b06fc-108">Esegui Set-CaseHoldPolicy <policyname> -RetryDistribution nel Centro Sicurezza e Conformità Powershell.</span><span class="sxs-lookup"><span data-stu-id="b06fc-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="b06fc-109">Per i dettagli vedere [Connettersi al Centro Sicurezza e Conformità PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="b06fc-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="b06fc-110">Per i passi necessari alla verifica di queste impostazioni e per le pratiche consigliate aggiuntive per mitigare e risolvere i problemi con i blocchi eDiscovery, consulta [Risoluzione dei problemi per gli errori nei blocchi eDiscovery](/microsoft-365/compliance/hold-distribution-errors).</span><span class="sxs-lookup"><span data-stu-id="b06fc-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="b06fc-111">Per informazioni sulla risoluzione di altri problemi comuni in eDiscovery, consulta [Investigare, risoluzione dei problemi e risolvere problemi comuni in eDiscovery](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span><span class="sxs-lookup"><span data-stu-id="b06fc-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
