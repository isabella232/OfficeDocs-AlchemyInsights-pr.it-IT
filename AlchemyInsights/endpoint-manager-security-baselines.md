---
title: EndPoint Manager - Baseline di sicurezza
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 4c8e03a817751ba7dc1710aed5a3e19c6e79db33
ms.sourcegitcommit: ae556b6b26974392ca68a68426a2b40967ae0071
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/07/2021
ms.locfileid: "58923558"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - Baseline di sicurezza

Le baseline di sicurezza sono gruppi preconfigurati di impostazioni di Windows che consentono di applicare le impostazioni di sicurezza consigliate dai team di sicurezza pertinenti. Queste baseline possono essere personalizzate in modo da fornire solo le impostazioni e i valori desiderati. Per altre informazioni sulle baseline di sicurezza, vedere [Usare le baseline di sicurezza per configurare i dispositivi Windows 10 in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Attualmente sono disponibili baseline per questi prodotti:

- Impostazioni di sicurezza di Windows MDM
- Sicurezza di Microsoft Defender per endpoint
- Microsoft Edge

Ognuna delle baseline viene aggiornata periodicamente e rilasciata in versioni incrementali. Ogni versione aggiunge e/o rimuove le impostazioni della versione precedente per garantire che la baseline soddisfi le indicazioni correnti. La console Baseline di sicurezza in Sicurezza degli endpoint consente di confrontare versioni diverse rendendo visibili le modifiche da una versione all'altra.

Per indicazioni su come modificare in modo più efficace la versione della baseline distribuita, vedere [Gestire i profili della baseline di sicurezza in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Dopo aver distribuito una baseline di sicurezza, è possibile monitorare lo stato della distribuzione ed esaminare le impostazioni a seconda dei dispositivi.

Poiché le baseline di sicurezza contengono molte impostazioni, è importante esaminare le modifiche alla configurazione ed eseguire test per assicurarsi che tutte le impostazioni siano appropriate per i dispositivi e le esigenze aziendali.

**Nota:** la visualizzazione dei dati dei report per le baseline può richiedere fino a 24 ore dalla distribuzione iniziale in un dispositivo e fino a 6 ore per ulteriori aggiornamenti. 

La causa più comune per cui un'impostazione della baseline non viene applicata è perché la stessa impostazione viene usata in un profilo diverso. Questo scenario può essere esaminato per un dispositivo specifico selezionando tale dispositivo nel nodo Stato dispositivo del profilo Baseline di sicurezza. Per informazioni dettagliate, vedere [Risolvere i conflitti per le baseline di sicurezza](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).