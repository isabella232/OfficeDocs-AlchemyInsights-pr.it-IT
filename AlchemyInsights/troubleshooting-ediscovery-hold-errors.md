---
title: Risoluzione dei problemi per gli errori nei blocchi ediscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 70f0302fd13324b6778390aeb0fe41ff5668d0d1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330784"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Risoluzione dei problemi per gli errori nei blocchi ediscovery

Si sono verificati problemi con i blocchi eDiscovery? Di seguito alcune procedure consigliate da tenere in considerazione: 

- Controlla lo stato di distribuzione del blocco.  Se lo stato è **On (in Sospeso)** o **Off (in Sospeso)**, attendere la completa distribuzione del blocco.
- Accorpa gli aggiornamenti del blocco eDiscovery in una singola richiesta invece di aggiornare il criterio ripetutamente per ogni transazione.
- Esegui Set-CaseHoldPolicy <policyname> -RetryDistribution nel Centro Sicurezza e Conformità Powershell. Per i dettagli vedere [Connettersi al Centro Sicurezza e Conformità PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell).

Per i passi necessari alla verifica di queste impostazioni e per le pratiche consigliate aggiuntive per mitigare e risolvere i problemi con i blocchi eDiscovery, consulta [Risoluzione dei problemi per gli errori nei blocchi eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/hold-distribution-errors).
Per informazioni sulla risoluzione di altri problemi comuni in eDiscovery, consulta [Investigare, risoluzione dei problemi e risolvere problemi comuni in eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).
