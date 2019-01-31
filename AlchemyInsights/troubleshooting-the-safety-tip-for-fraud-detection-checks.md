---
title: Risoluzione dei problemi la punta di sicurezza per il rilevamento di false controlla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 06a0b5b8d29052e6033de5938b8ea67ceabc9848
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658119"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="a5128-102">Risoluzione dei problemi la punta di sicurezza per il rilevamento di false controlla</span><span class="sxs-lookup"><span data-stu-id="a5128-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="a5128-p101">In caso di recupero di un suggerimento di sicurezza che informa che "il mittente non è riuscita i controlli di rilevamento di false e potrebbe non essere che vengano visualizzate come" e quindi il mittente non è riuscito a passare DKIM o SPF controlli di autenticazione. Il metodo migliore per risolvere questo problema è per il mittente autorizzare se stessi. Se il mittente invia per conto dell'utente, è necessario fornire le autorizzazioni aggiungendo l'indirizzo IP del mittente per il record SPF.</span><span class="sxs-lookup"><span data-stu-id="a5128-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="a5128-106">Per ulteriori informazioni, vedere [controlli di suggerimento rosso safety (sospetti) per il rilevamento di false](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="a5128-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="a5128-107">Ecco alcuni altri collegamenti che consentono di:</span><span class="sxs-lookup"><span data-stu-id="a5128-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="a5128-108">Utilizzo schema dei criteri di mittente (SPF) per impedire attacchi di spoofing del Office 365</span><span class="sxs-lookup"><span data-stu-id="a5128-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="a5128-109">Configurazione di SPF in Office 365 per evitare lo spoofing</span><span class="sxs-lookup"><span data-stu-id="a5128-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

