---
title: Risoluzione dei problemi relativi al blocco dei processi di importazione
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059846"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="ad430-102">Risoluzione dei problemi relativi al blocco dei processi di importazione</span><span class="sxs-lookup"><span data-stu-id="ad430-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="ad430-103">Se stai riscontrando problemi con il blocco o la mancata esecuzione dei servizi, esamina e prova quanto segue:</span><span class="sxs-lookup"><span data-stu-id="ad430-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="ad430-104">Controlla la dimensione del file PST.</span><span class="sxs-lookup"><span data-stu-id="ad430-104">Review the size of of the PST file.</span></span> <span data-ttu-id="ad430-105">La dimensione massima raccomandata dei file PST per l'importazione è 20 GB.</span><span class="sxs-lookup"><span data-stu-id="ad430-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="ad430-106">Se sospetti di avere saltato degli elementi danneggiati, esegui Scanpst.exe per diagnosticare e risolvere i problemi dei file PST.</span><span class="sxs-lookup"><span data-stu-id="ad430-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="ad430-107">Se riscontri un errore "MapiExceptionShutoffQuotaExceeded" durante l'importazione, assicurati che la capacità della cassetta postale di destinazione sia sufficiente per importare i tuoi file PST.</span><span class="sxs-lookup"><span data-stu-id="ad430-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="ad430-108">Per altre informazioni sulla risoluzione dei problemi dei processi di importazione dei file PST, vedi [Risoluzione dei problemi dei processi di importazione dei file PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="ad430-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="ad430-109">Per informazioni sulla risoluzione dei problemi di importazione dei file PST in Outlook, vedi [Risolvere i problemi di importazione dei file PST in Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="ad430-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>