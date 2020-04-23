---
title: Risoluzione dei problemi del suggerimento sulla sicurezza per i controlli di rilevamento delle frodi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759516"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Risoluzione dei problemi del suggerimento sulla sicurezza per i controlli di rilevamento delle frodi

Se si riceve un suggerimento per la sicurezza che indica che "il mittente ha superato i controlli di rilevamento delle frodi e potrebbe non essere quello che sembra", il mittente non ha superato i controlli di autenticazione DKIM o SPF. Il metodo migliore per risolvere questa operazione consiste nel consentire al mittente di autoautorizzarsi. Se il mittente sta inviando il proprio nome, è necessario autorizzarli aggiungendo l'indirizzo IP del mittente al record SPF.
  
Per ulteriori informazioni, vedere [Troubleshooting the Red (sospette) Safety Tip for Fraud Detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Di seguito sono riportati alcuni altri collegamenti che possono essere utili:
  
- [Utilizzo di Microsoft Sender Policy Framework (SPF) per impedire lo spoofing](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurare SPF per impedire lo spoofing](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
