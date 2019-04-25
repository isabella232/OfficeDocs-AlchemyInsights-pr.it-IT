---
title: Utilizzo delle applicazioni iOS VPP regola ID 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420488"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="23137-102">Utilizzo delle applicazioni di iOS VPP</span><span class="sxs-lookup"><span data-stu-id="23137-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="23137-103">Leggere [come gestire le app iOS acquistate tramite un programma di acquisto di volumi con Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) per informazioni sulle caratteristiche, i vincoli e i passaggi necessari per utilizzare il programma di acquisto dei volumi di Apple e il relativo supporto in Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="23137-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="23137-104">**Problemi comuni:** "È stata assegnata un'app iOS VPP ai miei utenti, ma l'installazione ha avuto esito negativo".</span><span class="sxs-lookup"><span data-stu-id="23137-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="23137-105">Questo può verificarsi se un singolo token VPP viene utilizzato su più provider di gestione dei dispositivi mobili.</span><span class="sxs-lookup"><span data-stu-id="23137-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="23137-106">I token VPP di Apple possono essere utilizzati solo con un solo provider.</span><span class="sxs-lookup"><span data-stu-id="23137-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="23137-107">Se è stato utilizzato un token VPP con più provider, è necessario caricare di nuovo il token in Intune.</span><span class="sxs-lookup"><span data-stu-id="23137-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="23137-108">L'installazione può anche avere esito negativo se il numero totale di installazioni supera il numero di licenze.</span><span class="sxs-lookup"><span data-stu-id="23137-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="23137-109">Per visualizzare un report di utilizzo per le licenze, accedere alla pagina **licenze app** per **dispositivi mobili** \> di Intune.</span><span class="sxs-lookup"><span data-stu-id="23137-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="23137-110">Per informazioni su come recuperare le licenze in uso, vedere [questo articolo.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="23137-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

