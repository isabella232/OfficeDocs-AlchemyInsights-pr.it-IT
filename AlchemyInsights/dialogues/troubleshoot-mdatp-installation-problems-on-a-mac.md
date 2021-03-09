---
title: Risolvere i problemi di installazione di MDATP in un Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568624"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="50d74-102">Risolvere i problemi di installazione di MDATP in un Mac</span><span class="sxs-lookup"><span data-stu-id="50d74-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="50d74-103">Se l'installazione manuale non riesce, nella pagina **Riepilogo** dell'installazione guidata viene visualizzato l'errore seguente:</span><span class="sxs-lookup"><span data-stu-id="50d74-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="50d74-104">"Si è verificato un errore durante l'installazione.</span><span class="sxs-lookup"><span data-stu-id="50d74-104">"An error occurred during installation.</span></span> <span data-ttu-id="50d74-105">Il programma di installazione ha riscontrato un errore che ha causato l'esito negativo dell'installazione.</span><span class="sxs-lookup"><span data-stu-id="50d74-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="50d74-106">Contattare il produttore del software per assistenza."</span><span class="sxs-lookup"><span data-stu-id="50d74-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="50d74-107">Per le distribuzioni MDM, la pagina mostra anche un errore di installazione generico.</span><span class="sxs-lookup"><span data-stu-id="50d74-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="50d74-108">Anche se non vengono visualizzati errori esatti per gli utenti finali, microsoft mantiene un file di registro con lo stato di avanzamento dell'installazione, in **/Library/Logs/Microsoft/mdatp/install.log.**</span><span class="sxs-lookup"><span data-stu-id="50d74-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="50d74-109">Ogni sessione di installazione viene aggiunta a questo file di registro.</span><span class="sxs-lookup"><span data-stu-id="50d74-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="50d74-110">Per output solo per l'ultima sessione di installazione, utilizzare `sed` .</span><span class="sxs-lookup"><span data-stu-id="50d74-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="50d74-111">Per altre informazioni, vedere Risolvere i problemi di installazione [per Microsoft Defender ATP per Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="50d74-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
