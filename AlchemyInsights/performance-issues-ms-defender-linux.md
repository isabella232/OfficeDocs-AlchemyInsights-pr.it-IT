---
title: Problemi di prestazioni per Microsoft Defender per endpoint su Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783433"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="5dd04-102">Problemi di prestazioni per Microsoft Defender per endpoint su Linux</span><span class="sxs-lookup"><span data-stu-id="5dd04-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="5dd04-103">In questo articolo vengono specificati i passaggi per l'identificazione dei problemi di prestazioni per Microsoft Defender per endpoint su Linux.</span><span class="sxs-lookup"><span data-stu-id="5dd04-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="5dd04-104">Per prima cosa, è importante verificare se problema riscontrato sia risolvibile nella [versione più recente](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="5dd04-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="5dd04-105">Per avviare l'indagine, vedere [Risoluzione dei problemi di prestazioni per Microsoft Defender per endpoint su Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span><span class="sxs-lookup"><span data-stu-id="5dd04-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="5dd04-106">Esclusioni</span><span class="sxs-lookup"><span data-stu-id="5dd04-106">Exclusions</span></span>

<span data-ttu-id="5dd04-107">Le esclusioni possono aiutare a ridurre i problemi di prestazioni.</span><span class="sxs-lookup"><span data-stu-id="5dd04-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="5dd04-108">Rivedere le esclusioni prima di iniziare, così che qualsiasi rischio aggiuntivo sia noto e documentato.</span><span class="sxs-lookup"><span data-stu-id="5dd04-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="5dd04-109">Per ulteriori informazioni, vedere [Configurare e convalidare le esclusioni per Microsoft Defender per endpoint su Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="5dd04-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="5dd04-110">Se si dispone di più file e cartelle da escludere sullo stesso punto di montaggio, potrebbe essere più facile escludere tale punto di montaggio.</span><span class="sxs-lookup"><span data-stu-id="5dd04-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="5dd04-111">A partire dalla release 101.22.80 di febbraio, è possibile escludere un intero punto di montaggio.</span><span class="sxs-lookup"><span data-stu-id="5dd04-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="5dd04-112">Ad esempio, se /mnt/backup è un punto di montaggio, è possibile aggiungere /mnt/backup all'elenco di esclusione eseguendo questo domando:</span><span class="sxs-lookup"><span data-stu-id="5dd04-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="5dd04-113">**Nota**: l'aggiunta di esclusioni aumenta il rischio della mancata identificazione di malware e dovrebbe essere gestita e implementata con attenzione.</span><span class="sxs-lookup"><span data-stu-id="5dd04-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="5dd04-114">Servono altre informazioni?</span><span class="sxs-lookup"><span data-stu-id="5dd04-114">Need Help?</span></span>

<span data-ttu-id="5dd04-115">Per poter ricevere la migliore assistenza, è necessario fornire i dati di diagnostica prima di aprire un caso di supporto.</span><span class="sxs-lookup"><span data-stu-id="5dd04-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
