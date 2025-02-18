---
title: Distribuzione di Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9139"
- "11088"
- "9005291"
- "9006490"
ms.openlocfilehash: b8f2cc0164fd656279aed456a7f9c48ba3442e78
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314776"
---
# <a name="deploy-microsoft-edge"></a>Distribuzione di Microsoft Edge

Dopo aver definito i criteri e aver terminato i test di compatibilità delle app iniziali, è tutto pronto per la distribuzione al gruppo pilota. La distribuzione al gruppo pilota consente di ricevere feedback e correggere i problemi prima dell'implementazione di Microsoft Edge nell'intera organizzazione.

Per la distribuzione di Microsoft Edge, sono disponibili gli strumenti seguenti:

- [Microsoft Intune per Windows](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge) o [Microsoft Intune per macOS](https://docs.microsoft.com/mem/intune/apps/apps-edge-macos)
- [Configuration Manager](https://docs.microsoft.com/DeployEdge/deploy-edge-with-configuration-manager)
- Un altro strumento che usa il [file MSI per Microsoft Edge](https://www.microsoft.com/edge/business/download)

**Convalidare la distribuzione**

Dopo la distribuzione del gruppo pilota, è consigliabile acquisire feedback degli utenti. Tenere in considerazione gli aspetti seguenti:
- **Compatibilità**: identificare i siti appartenenti all'elenco dei siti modalità Enterprise che non sono stati identificati durante l'individuazione dei siti.
- **Configurazione criteri**: assicurarsi che gli utenti possano usare le funzionalità principali ed eseguire le attività seguendo le linee guida di sicurezza.
- **Facilità d'uso e nuove funzionalità**: identificare le aree in cui è necessario sviluppare e distribuire la formazione in base alle domande dell'utente.

**Distribuzione ampia di Microsoft Edge**

Dopo aver distribuito il progetto pilota e aggiornato il piano di distribuzione con le informazioni apprese, è tutto pronto per eseguire una distribuzione completa di Microsoft Edge a tutti gli utenti. Congratulazioni!

