---
title: Posta elettronica in uscita alla cartella posta indesiderata
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 869cd3d9fb8e5fce291244e4a39754d074b11358
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511728"
---
# <a name="outbound-email-to-junk-email-folder"></a>Posta elettronica in uscita alla cartella posta indesiderata

Se i messaggi in uscita vengono contrassegnati come posta indesiderata, eseguire le operazioni seguenti:

- Se non è stato già, è consigliabile [configurare le notifiche sui criteri di posta indesiderata in uscita](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).

- Utilizzare la [traccia dei messaggi](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) per verificare se il messaggio in uscita ha il valore di evento **posta indesiderata** con l'ulteriore dettaglio: **utilizza pool di recapito ad alto rischio**.

  Per questi messaggi, controllare il contenuto del messaggio per vedere cosa può essere considerato come posta indesiderata. Ad esempio, le firme possono talvolta causare problemi a molti utenti.

  Se si dispone di più esempi di messaggi in uscita legittimi contrassegnati come posta indesiderata, aprire un ticket di supporto e chiedere all'agente di supporto di inviare i messaggi come falsi positivi ai nostri analisti di posta indesiderata. Prepararsi a fornire messaggi di esempio che includano tutte le intestazioni dei messaggi.
