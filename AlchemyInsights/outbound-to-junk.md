---
title: Posta elettronica in uscita nella cartella Posta indesiderata
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 52aa5aa86848fa92ac082e8f672f9f501cd97cf2f3db9c40fa745aa8ebccfbb1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54096662"
---
# <a name="outbound-email-to-junk-email-folder"></a>Posta elettronica in uscita nella cartella Posta indesiderata

Se i messaggi in uscita vengono contrassegnati come posta indesiderata, eseguire la procedura seguente:

- Se non l'hai già fatto, valuta la possibilità di configurare le notifiche dei criteri [di posta indesiderata in uscita.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)

- Utilizzare [traccia dei messaggi](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) per verificare se il messaggio in uscita ha il valore di evento **Spam** con il dettaglio aggiuntivo: Use high risk **delivery pool**.

  Per questi messaggi, controllare il contenuto del messaggio per vedere cosa potrebbe essere considerato posta indesiderata. Ad esempio, le firme a volte possono causare problemi a molti utenti.

  Se si dispone di più esempi di messaggi in uscita legittimi contrassegnati come posta indesiderata, aprire un ticket di supporto e chiedere all'agente di supporto di inviare i messaggi come falsi positivi ai nostri analisti della posta indesiderata. Prepararsi a fornire messaggi di esempio che includono tutte le intestazioni dei messaggi.
