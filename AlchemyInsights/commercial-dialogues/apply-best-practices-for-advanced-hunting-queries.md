---
title: Applicare le procedure consigliate per le query di ricerca avanzate
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736857"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="53dc5-102">Applicare le procedure consigliate per le query di ricerca avanzate</span><span class="sxs-lookup"><span data-stu-id="53dc5-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="53dc5-103">Per ottenere risultati più veloci ed evitare timeout durante l'esecuzione di query complesse, applicare le procedure consigliate seguenti:</span><span class="sxs-lookup"><span data-stu-id="53dc5-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="53dc5-104">Quando si provano nuove query, utilizzare sempre un limite per evitare di ottenere set di risultati estremamente grandi.</span><span class="sxs-lookup"><span data-stu-id="53dc5-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="53dc5-105">Utilizzare inoltre `count` per effettuare una valutazione iniziale delle dimensioni del set di risultati.</span><span class="sxs-lookup"><span data-stu-id="53dc5-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="53dc5-106">Usare prima i filtri del periodo.</span><span class="sxs-lookup"><span data-stu-id="53dc5-106">Use time filters first.</span></span> <span data-ttu-id="53dc5-107">Idealmente, limitare le query a sette giorni.</span><span class="sxs-lookup"><span data-stu-id="53dc5-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="53dc5-108">All'inizio di una query, subito dopo il filtro temporale, aggiungere i filtri previsti per rimuovere la maggior parte dei dati.</span><span class="sxs-lookup"><span data-stu-id="53dc5-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="53dc5-109">Quando cerchi token completi, usa `has` l'operatore anziché `contains` .</span><span class="sxs-lookup"><span data-stu-id="53dc5-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="53dc5-110">Eseguire una ricerca in una colonna specifica anziché in tutte le colonne.</span><span class="sxs-lookup"><span data-stu-id="53dc5-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="53dc5-111">Quando si uniscono tabelle, specificare innanzitutto la tabella con un numero minore di righe.</span><span class="sxs-lookup"><span data-stu-id="53dc5-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="53dc5-112">`project` solo le colonne necessarie delle tabelle unite.</span><span class="sxs-lookup"><span data-stu-id="53dc5-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="53dc5-113">Per ulteriori informazioni, vedere [Advanced hunting query best practices.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="53dc5-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
