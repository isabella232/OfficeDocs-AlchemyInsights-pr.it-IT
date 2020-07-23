---
title: Conflitti con SourceAnchor, ProxyAddress, UserPrincipalName
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1699"
- "1300022"
ms.openlocfilehash: 826dfe9e5c7d24ff5186a94e1ada4dad536e7edd
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186126"
---
# <a name="conflicts-with-sourceanchor-proxyaddress-userprincipalname"></a><span data-ttu-id="9a74b-102">Conflitti con SourceAnchor, ProxyAddress, UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9a74b-102">Conflicts with SourceAnchor, ProxyAddress, UserPrincipalName</span></span>

<span data-ttu-id="9a74b-103">Se durante una sincronizzazione si ricevono errori simili a "Nella directory esiste già un oggetto sincronizzato con lo stesso valore di ProxyAddress o UserPrincipalName", vedere [Diagnosticare e risolvere gli errori di sincronizzazione degli attributi duplicati](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span><span class="sxs-lookup"><span data-stu-id="9a74b-103">If you receive errors during a synchronization such as "A synchronized object with the same ProxyAddress or UserPrincipalName exists in your directory", see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>

<span data-ttu-id="9a74b-104">Inoltre, è consigliabile abilitare la resilienza degli attributi duplicati.</span><span class="sxs-lookup"><span data-stu-id="9a74b-104">Also, consider enabling duplicate attribute resiliency.</span></span> <span data-ttu-id="9a74b-105">Per altre informazioni, vedere [Sincronizzazione delle identità e resilienza degli attributi duplicati](https://aka.ms/duplicateattributeresiliency).</span><span class="sxs-lookup"><span data-stu-id="9a74b-105">For more info, see [Identity synchronization and duplicate attribute resiliency](https://aka.ms/duplicateattributeresiliency).</span></span>