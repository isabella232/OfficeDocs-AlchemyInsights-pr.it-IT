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
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29936364"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Risoluzione dei problemi la punta di sicurezza per il rilevamento di false controlla



In caso di recupero di un suggerimento di sicurezza che informa che "il mittente non è riuscita i controlli di rilevamento di false e potrebbe non essere che vengano visualizzate come" e quindi il mittente non è riuscito a passare DKIM o SPF controlli di autenticazione. Il metodo migliore per risolvere questo problema è per il mittente autorizzare se stessi. Se il mittente invia per conto dell'utente, è necessario fornire le autorizzazioni aggiungendo l'indirizzo IP del mittente per il record SPF.
  
Per ulteriori informazioni, vedere [controlli di suggerimento rosso safety (sospetti) per il rilevamento di false](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) . 
  
Ecco alcuni altri collegamenti che consentono di:
  
- [Utilizzo schema dei criteri di mittente (SPF) per impedire attacchi di spoofing del Office 365](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [Configurazione di SPF in Office 365 per evitare lo spoofing](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

