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
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="931fb-102">Problemi con l’esecuzione dell’onboarding di computer</span><span class="sxs-lookup"><span data-stu-id="931fb-102">Issues with onboarding machines</span></span>

<span data-ttu-id="931fb-103">Potrebbero verificarsi problemi per eseguire l’onboarding di computer al servizio MDATP.</span><span class="sxs-lookup"><span data-stu-id="931fb-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="931fb-104">Se è possibile accedere al computer dell'utente finale, effettuare i seguenti passaggi:</span><span class="sxs-lookup"><span data-stu-id="931fb-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="931fb-105">Scaricare lo strumento di diagnostica [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="931fb-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="931fb-106">Estrarre ed eseguire MDATPAnalyzer.cmd.</span><span class="sxs-lookup"><span data-stu-id="931fb-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="931fb-107">Individuare il log di diagnostica nella cartella MDATPClientAnalyzerResult, la stessa cartella in cui è stato scaricato Analyzer.</span><span class="sxs-lookup"><span data-stu-id="931fb-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="931fb-108">Controllare il file di log, MDATPClientAnalyzer.txt, per trovare problemi di connettività o di impostazioni proxy Internet.</span><span class="sxs-lookup"><span data-stu-id="931fb-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>