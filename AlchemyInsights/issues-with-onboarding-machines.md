---
title: Problemi con l’onboarding delle macchine a Microsoft Defender per Endpoint
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
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901571"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="b2cf6-102">Problemi con l’onboarding delle macchine a Microsoft Defender per Endpoint</span><span class="sxs-lookup"><span data-stu-id="b2cf6-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="b2cf6-103">Potrebbero verificarsi problemi con l’onboarding delle macchine al servizio MDE.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="b2cf6-104">Se è possibile accedere al computer dell'utente finale, effettuare i seguenti passaggi:</span><span class="sxs-lookup"><span data-stu-id="b2cf6-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="b2cf6-105">Scaricare la versione di anteprima più recente dello strumento di diagnostica [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="b2cf6-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="b2cf6-106">Fare clic con il pulsante destro del mouse su **MDEClientAnalyzer.cmd** e selezionare “Esegui come amministratore”.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="b2cf6-107">Seguire tutte le indicazioni suggerite in **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="b2cf6-108">Per registri più dettagliati, rivedere la sottocartella creata denominata **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="b2cf6-109">Se sono necessarie ulteriori indicazioni, contattare il [supporto di Microsoft Defender per Endpoint](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) e fornire il file MDEClientAnalyzerResult.zip risultante per l’analisi.</span><span class="sxs-lookup"><span data-stu-id="b2cf6-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
