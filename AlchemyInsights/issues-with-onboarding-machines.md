---
title: Problemi con l’esecuzione dell’onboarding di computer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676886"
---
# <a name="issues-with-onboarding-machines"></a>Problemi con l’esecuzione dell’onboarding di computer

Potrebbero verificarsi problemi per eseguire l’onboarding di computer al servizio MDATP. Se è possibile accedere al computer dell'utente finale, effettuare i seguenti passaggi:

1. Scaricare lo strumento di diagnostica [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer).
2. Estrarre ed eseguire MDATPAnalyzer.cmd.
3. Individuare il log di diagnostica nella cartella MDATPClientAnalyzerResult, la stessa cartella in cui è stato scaricato Analyzer.
4. Controllare il file di log, MDATPClientAnalyzer.txt, per trovare problemi di connettività o di impostazioni proxy Internet.