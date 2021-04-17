---
title: Risoluzione dei problemi relativi al suggerimento per la sicurezza per i controlli di rilevamento delle frodi
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834735"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Risoluzione dei problemi relativi al suggerimento per la sicurezza per i controlli di rilevamento delle frodi

Se si riceve un suggerimento per la sicurezza che indica che il mittente non ha superato i controlli di rilevamento delle frodi e potrebbe non essere quello che sembra essere", il mittente non è riuscito a superare i controlli di autenticazione DKIM o SPF. Il metodo migliore per risolvere il problema è che il mittente si autorizzi. Se il mittente invia per conto dell'utente, è necessario autorizzarlo aggiungendo l'indirizzo IP del mittente al record SPF.
  
Vedi [Risoluzione dei problemi del suggerimento di sicurezza rosso (sospetto) per i controlli di rilevamento delle frodi](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) per altre info.
  
Ecco alcuni altri collegamenti utili:
  
- [Come Microsoft usa SPF (Sender Policy Framework) per impedire lo spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurazione di SPF per evitare lo spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
