---
title: Problemi con l’esecuzione dell’onboarding di computer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/15/2020
ms.locfileid: "45139026"
---
# <a name="issues-with-onboarding-machines"></a>Problemi con l’esecuzione dell’onboarding di computer

Potrebbero verificarsi problemi per eseguire l’onboarding di computer al servizio MDATP. Se è possibile accedere al computer dell'utente finale, effettuare i seguenti passaggi:

1. Scaricare lo strumento di diagnostica [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer).
2. Estrarre ed eseguire MDATPAnalyzer.cmd.
3. Individuare il log di diagnostica nella cartella MDATPClientAnalyzerResult, la stessa cartella in cui è stato scaricato Analyzer.
4. Controllare il file di log, MDATPClientAnalyzer.txt, per trovare problemi di connettività o di impostazioni proxy Internet.