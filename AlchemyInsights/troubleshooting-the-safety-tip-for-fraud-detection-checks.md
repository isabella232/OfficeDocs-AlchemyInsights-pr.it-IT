---
title: Risoluzione dei problemi suggerimento per la sicurezza per i controlli di rilevamento delle frodi
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955970"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Risoluzione dei problemi suggerimento per la sicurezza per i controlli di rilevamento delle frodi

Se si riceve un suggerimento per la sicurezza che indica che il mittente non ha superato i controlli di rilevamento delle frodi e potrebbe non essere chi sembra essere", il mittente non è riuscito a superare i controlli di autenticazione DKIM o SPF. Il metodo migliore per risolvere il problema è che il mittente si autorizzi. Se il mittente invia per conto dell'utente, è necessario autorizzarlo aggiungendo l'indirizzo IP del mittente al record SPF.
  
Per altre informazioni, vedi Risoluzione dei problemi relativi ai controlli di [rilevamento delle frodi suggerimento per la sicurezza](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) rosso (sospetto).
  
Ecco alcuni altri collegamenti utili:
  
- [Come Microsoft usa SPF (Sender Policy Framework) per impedire lo spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Configurazione di SPF per evitare lo spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
