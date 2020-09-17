---
title: Problema dello spooler di stampa risolto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801845"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="11577-102">Problema dello spooler di stampa risolto</span><span class="sxs-lookup"><span data-stu-id="11577-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="11577-103">Se il dispositivo è stato aggiornato con Windows 10, **build sistema operativo 19041.329**, potrebbe riscontrarsi un problema che non consente la stampa con alcune stampanti.</span><span class="sxs-lookup"><span data-stu-id="11577-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="11577-104">Lo spooler di stampa potrebbe generare un errore o chiudersi in modo imprevisto durante il tentativo di stampa e la stampante interessata non genera output.</span><span class="sxs-lookup"><span data-stu-id="11577-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="11577-105">Il problema è stato risolto con la build del sistema operativo **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="11577-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="11577-106">**Indagine in corso**</span><span class="sxs-lookup"><span data-stu-id="11577-106">**Ongoing investigation**</span></span>

<span data-ttu-id="11577-107">Il file Local Security Authority Subsystem Service (LSASS - **Isass.exe**) potrebbe presentare problemi in alcuni dispositivi e restituire il messaggio di errore "Processo di sistema critico, C:\WINDOWS\system32\Isass.exe, non riuscito con codice di stato c0000008.</span><span class="sxs-lookup"><span data-stu-id="11577-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="11577-108">Riavviare il computer.".</span><span class="sxs-lookup"><span data-stu-id="11577-108">The machine must now be restarted".</span></span>  <span data-ttu-id="11577-109">**Microsoft si sta occupando del problema e fornirà un aggiornamento in una delle prossime versioni.**</span><span class="sxs-lookup"><span data-stu-id="11577-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="11577-110">Per altre informazioni, consultare l'articolo sui [problemi noti di Windows 10 versione 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="11577-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>