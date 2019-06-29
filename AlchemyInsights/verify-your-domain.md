---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 5bd6c32a246db9dfcdb475368ade0441df4dc9c3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365421"
---
# <a name="verify-your-domain"></a><span data-ttu-id="241a7-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="241a7-102">Verify your domain</span></span>

 <span data-ttu-id="241a7-103">**Il record probabilmente non è stato aggiornato su Internet.**</span><span class="sxs-lookup"><span data-stu-id="241a7-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="241a7-104">In genere, è necessario solo qualche minuto perché sia possibile visualizzare il nuovo record, ma a volte può richiedere fino a poche ore.</span><span class="sxs-lookup"><span data-stu-id="241a7-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="241a7-105">Se si è già aspettato tanto, verificare di aver copiato e incollato il valore esatto nel record di verifica TXT nell'host DNS.</span><span class="sxs-lookup"><span data-stu-id="241a7-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="241a7-106">Un problema comune non include la parte "MS =" del record.</span><span class="sxs-lookup"><span data-stu-id="241a7-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="241a7-107">Ci serve anche questo!</span><span class="sxs-lookup"><span data-stu-id="241a7-107">We need that too!</span></span>

- <span data-ttu-id="241a7-108">Presso alcuni host DNS è necessario eseguire un ulteriore passaggio per salvare il file di zona (in cui è archiviato il record DNS) in modo che venga aggiornato su Internet.</span><span class="sxs-lookup"><span data-stu-id="241a7-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="241a7-109">Verificare di avere salvato le modifiche affinché Office 365 possa visualizzare e verificare il record.</span><span class="sxs-lookup"><span data-stu-id="241a7-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
