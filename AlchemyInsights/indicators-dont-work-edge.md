---
title: Gli indicatori non funzionano con il browser Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651509"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Gli indicatori non funzionano con il browser Microsoft Edge

Dopo la creazione, l'indicatore non viene rispettato da Microsoft Edge (SmartScreen). Per altre informazioni, vedere [Creare indicatori per IP e URL/domini](/microsoft-365/security/defender-endpoint/indicator-ip-domain).

## <a name="step-1-ensure-the-following"></a>Passaggio 1: verificare quanto segue

- Verificare che l'indicatore sia corretto (nessun errore di digitazione in IP/URL, azione corretta, gruppi RBAC corretti).
- Attendere almeno 2 ore dopo la creazione dell'indicatore per prendere in considerazione l'eventuale latenza.
- Verificare che sia stato eseguito l’onboarding dei sistemi in Microsoft Defender per endpoint.
- Verificare che i sistemi riescano a comunicare con il cloud.
- Per verificare che SmartScreen sia abilitato e raggiungibile, accedere al [sito di test](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Passaggio 2: risolvere il problema potenziale

- Verificare che il client soddisfi i requisiti. Per informazioni dettagliate, vedere [Creare indicatori per IP e URL/domini](/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- Verificare di eseguire la versione più recente del Web browser Microsoft Edge. Per informazioni sulla versione più recente, vedere [Scopri quale versione di Microsoft Edge possiedi](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Riavviare il Web browser Microsoft Edge.
- Passare al sito per cui è stato configurato un indicatore. Se il sito non viene visualizzato come previsto, procedere al passaggio 3. 

## <a name="step-3-collect-data"></a>Passaggio 3: raccogliere dati

- Raccogliere i dati di diagnostica **MDEClientAnalyzer**. Per istruzioni, vedere [Problemi con l’onboarding delle macchine a Microsoft Defender per endpoint](issues-with-onboarding-machines.md).
- Se si ha familiarità con l'installazione e la raccolta di una traccia di Fiddler, vedere [Telerik Fiddler](http://www.telerik.com/fiddler).
- Se si preferisce ottenere indicazioni dal supporto tecnico Microsoft, selezionare l'icona Supporto di seguito per aprire un caso di supporto.
