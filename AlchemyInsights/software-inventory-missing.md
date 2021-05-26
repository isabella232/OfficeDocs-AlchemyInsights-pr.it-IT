---
title: Inventario software mancante o non corretto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658052"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="80e01-102">Inventario software mancante o non corretto</span><span class="sxs-lookup"><span data-stu-id="80e01-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="80e01-103">L'inventario software nella funzionalità per la gestione di minacce e vulnerabilità è un elenco di software noti dell'organizzazione con enumerazioni CPE ( Common Platform Enumeration) ufficiali.</span><span class="sxs-lookup"><span data-stu-id="80e01-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="80e01-104">I prodotti software senza CPE ufficiale non hanno vulnerabilità pubblicate.</span><span class="sxs-lookup"><span data-stu-id="80e01-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="80e01-105">L'inventario include anche dettagli come il nome del fornitore, il numero di punti deboli, le minacce e il numero di dispositivi esposti.</span><span class="sxs-lookup"><span data-stu-id="80e01-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="80e01-106">Le modifiche al software nei dispositivi vengono in genere rispecchiate portali di sicurezza entro due ore.</span><span class="sxs-lookup"><span data-stu-id="80e01-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="80e01-107">A volte, tuttavia, può essere necessario più tempo.</span><span class="sxs-lookup"><span data-stu-id="80e01-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="80e01-108">Attualmente non è possibile forzare una sincronizzazione, la valutazione è continua.</span><span class="sxs-lookup"><span data-stu-id="80e01-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="80e01-109">Se è stata apportata una modifica al software e la modifica non è rispecchiata in modo accurato in TVM dopo 5 ore, seguire questa procedura:</span><span class="sxs-lookup"><span data-stu-id="80e01-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="80e01-110">Consultare la sezione delle prove software per capire come è stato rilevato il software.</span><span class="sxs-lookup"><span data-stu-id="80e01-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="80e01-111">Assicurarsi che il software sia supportato.</span><span class="sxs-lookup"><span data-stu-id="80e01-111">Make sure that the software is supported.</span></span> <span data-ttu-id="80e01-112">Il software può essere visibile solo a livello di dispositivo, anche se attualmente non è supportato dalla gestione di minacce e vulnerabilità.</span><span class="sxs-lookup"><span data-stu-id="80e01-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="80e01-113">Tuttavia, sono disponibili solo dati limitati.</span><span class="sxs-lookup"><span data-stu-id="80e01-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="80e01-114">Per la procedura da seguire per segnalare l'imprecisione del portale, vedere [Imprecisione dei report](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="80e01-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="80e01-115">**Nota**: la segnalazione di un'inesattezza dal portale MDE è un canale di comunicazione con i tecnici unidirezionale.</span><span class="sxs-lookup"><span data-stu-id="80e01-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="80e01-116">Se il problema è urgente, aprire un ticket di supporto.</span><span class="sxs-lookup"><span data-stu-id="80e01-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="80e01-117">Per ulteriori informazioni, vedere [Inventario software: gestione di minacce e vulnerabilità](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span><span class="sxs-lookup"><span data-stu-id="80e01-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>