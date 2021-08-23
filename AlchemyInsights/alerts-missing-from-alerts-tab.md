---
title: Avvisi mancanti dalla scheda Avvisi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362386"
---
# <a name="alerts-missing-from-alerts-tab"></a>Avvisi mancanti dalla scheda Avvisi

La **scheda Avvisi** funziona in base alla configurazione e ai criteri attivati dal portale di governance delle app nel tenant. Anche i criteri predefiniti in Governance app devono essere attivati per consentire il flusso dei segnali nella **scheda** Avvisi. 

Verificare che l'avviso sia stato generato:

1. Vai a Criteri [di](https://compliance.microsoft.com/m365appprotection?viewid=policies) governance delle app e verifica di aver creato almeno un criterio attivo o di controllo.

1. Selezionare il criterio e quindi selezionare Modifica **nel** riquadro a comparsa. 

1. Controlla la configurazione dei criteri per verificare che un avviso sia stato generato in base a un evento di criteri avviato più di 24 ore fa.

Per altre informazioni sugli avvisi in Governance delle app, vedi Introduzione al rilevamento e alla correzione delle minacce [delle app.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)