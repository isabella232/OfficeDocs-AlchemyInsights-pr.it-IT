---
title: Risoluzione dei problemi del suggerimento sulla sicurezza per i controlli di rilevamento delle frodi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658414"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Risoluzione dei problemi del suggerimento sulla sicurezza per i controlli di rilevamento delle frodi

Se si riceve un suggerimento per la sicurezza che indica che "il mittente ha superato i controlli di rilevamento delle frodi e potrebbe non essere quello che sembra", il mittente non ha superato i controlli di autenticazione DKIM o SPF. Il metodo migliore per risolvere questa operazione consiste nel consentire al mittente di autoautorizzarsi. Se il mittente sta inviando il proprio nome, è necessario autorizzarli aggiungendo l'indirizzo IP del mittente al record SPF.
  
Per ulteriori informazioni, vedere [Troubleshooting the Red (sospette) Safety Tip for Fraud Detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .
  
Di seguito sono riportati alcuni altri collegamenti che possono essere utili:
  
- [Utilizzo di Microsoft Sender Policy Framework (SPF) per impedire lo spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurazione di SPF per evitare lo spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
