---
title: Risoluzione dei problemi la punta di sicurezza per il rilevamento di false controlla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475839"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Risoluzione dei problemi la punta di sicurezza per il rilevamento di false controlla

In caso di recupero di un suggerimento di sicurezza che informa che "il mittente non è riuscita i controlli di rilevamento di false e potrebbe non essere che vengano visualizzate come" e quindi il mittente non è riuscito a passare DKIM o SPF controlli di autenticazione. Il metodo migliore per risolvere questo problema è per il mittente autorizzare se stessi. Se il mittente invia per conto dell'utente, è necessario fornire le autorizzazioni aggiungendo l'indirizzo IP del mittente per il record SPF.
  
Per ulteriori informazioni, vedere [controlli di suggerimento rosso safety (sospetti) per il rilevamento di false](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) . 
  
Ecco alcuni altri collegamenti che consentono di:
  
- Utilizzo di Sender Policy Framework (SPF) in Office 365 per impedire lo spoofing
    
- [Configurazione di SPF in Office 365 per evitare lo spoofing](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

