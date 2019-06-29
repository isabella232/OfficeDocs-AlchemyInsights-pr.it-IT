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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Risoluzione dei problemi del suggerimento sulla sicurezza per i controlli di rilevamento delle frodi

Se si riceve un suggerimento per la sicurezza che indica che "il mittente ha superato i controlli di rilevamento delle frodi e potrebbe non essere quello che sembra", il mittente non ha superato i controlli di autenticazione DKIM o SPF. Il metodo migliore per risolvere questa operazione consiste nel consentire al mittente di autoautorizzarsi. Se il mittente sta inviando il proprio nome, è necessario autorizzarli aggiungendo l'indirizzo IP del mittente al record SPF.
  
Per ulteriori informazioni, vedere [Troubleshooting the Red (sospette) Safety Tip for Fraud Detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Di seguito sono riportati alcuni altri collegamenti che possono essere utili:
  
- [Modalità di utilizzo di Office 365 (Sender Policy Framework) per impedire lo spoofing](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurazione di SPF in Office 365 per evitare lo spoofing](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
