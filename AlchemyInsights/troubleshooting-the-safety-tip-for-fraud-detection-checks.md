---
title: Risoluzione dei problemi del suggerimento sulla sicurezza per i controlli di rilevamento delle frodi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353253"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="c4ad7-102">Risoluzione dei problemi del suggerimento sulla sicurezza per i controlli di rilevamento delle frodi</span><span class="sxs-lookup"><span data-stu-id="c4ad7-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="c4ad7-103">Se si riceve un suggerimento per la sicurezza che indica che "il mittente ha superato i controlli di rilevamento delle frodi e potrebbe non essere quello che sembra", il mittente non ha superato i controlli di autenticazione DKIM o SPF.</span><span class="sxs-lookup"><span data-stu-id="c4ad7-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="c4ad7-104">Il metodo migliore per risolvere questa operazione consiste nel consentire al mittente di autoautorizzarsi.</span><span class="sxs-lookup"><span data-stu-id="c4ad7-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="c4ad7-105">Se il mittente sta inviando il proprio nome, è necessario autorizzarli aggiungendo l'indirizzo IP del mittente al record SPF.</span><span class="sxs-lookup"><span data-stu-id="c4ad7-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="c4ad7-106">Per ulteriori informazioni, vedere [Troubleshooting the Red (sospette) Safety Tip for Fraud Detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="c4ad7-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="c4ad7-107">Di seguito sono riportati alcuni altri collegamenti che possono essere utili:</span><span class="sxs-lookup"><span data-stu-id="c4ad7-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="c4ad7-108">Modalità di utilizzo di Office 365 (Sender Policy Framework) per impedire lo spoofing</span><span class="sxs-lookup"><span data-stu-id="c4ad7-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="c4ad7-109">Configurazione di SPF in Office 365 per evitare lo spoofing</span><span class="sxs-lookup"><span data-stu-id="c4ad7-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
