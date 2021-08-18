---
title: Controllo dello stato del sensore di Defender per endpoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: 903d64a59d3bf870572c3c643e3d9cb801b571cb
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321079"
---
# <a name="defender-endpoint-check-sensor-status"></a>Controllo dello stato del sensore di Defender per endpoint

Il riquadro **Dispositivi con problemi di sensore** si trova nel dashboard Operazioni di sicurezza. Questo riquadro fornisce informazioni sulla capacità del singolo dispositivo di fornire dati sul sensore e comunicare con il servizio Defender per endpoint. Segnala quanti dispositivi richiedono attenzione e aiuta a identificare i dispositivi problematici per intraprendere le azioni volte a correggere i problemi noti.

Due indicatori di stato nel riquadro forniscono informazioni sul numero di dispositivi che non segnalano correttamente al servizio:

- **Configurazione non corretta** Dispositivi che potrebbero segnalare parzialmente i dati del sensore al servizio Defender per endpoint e contenere errori di configurazione da correggere.
- **Inattivi** Dispositivi che hanno interrotto la segnalazione al servizio Defender per endpoint per più di sette giorni nell'ultimo mese.

Facendo clic su uno dei gruppi, si viene indirizzati all'elenco Dispositivi, filtrato in base alle scelte effettuate. È possibile filtrare l'elenco Dispositivi in base allo stato di integrità come segue:

- **Attivi** Dispositivi che segnalano attivamente al servizio Defender per endpoint.
- **Configurazione non corretta** Dispositivi che potrebbero segnalare parzialmente i dati del sensore al servizio Defender per endpoint e contengono errori di configurazione da correggere. Nei dispositivi non configurati correttamente possono verificarsi uno o più dei seguenti problemi:

    - Nessun dato del sensore: i dispositivi hanno smesso di inviare dati del sensore. Il dispositivo può generare avvisi limitati.
    - Comunicazioni con problemi: sono presenti problemi di comunicazione con il dispositivo. L'invio di file per un'analisi approfondita, il blocco dei file, l'isolamento del dispositivo dalla rete e altre azioni che richiedono la comunicazione con il dispositivo potrebbero non funzionare.
- **Inattivi** Dispositivi che hanno interrotto la segnalazione al servizio Defender per endpoint.

È possibile scaricare l'intero elenco in formato CSV usando la funzionalità Esporta.

Per altre informazioni, vedere [Controllare lo stato di integrità del sensore in Microsoft Defender per endpoint](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/check-sensor-status).

Per altre informazioni su ciò che ha causato l'inattività o la configurazione non corretta di un dispositivo, vedere [Correggere i sensori non integri in Microsoft Defender per endpoint](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).
