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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736926"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="677cc-102">Risolvere i problemi di installazione di MDATP in un Mac</span><span class="sxs-lookup"><span data-stu-id="677cc-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="677cc-103">Se l'installazione manuale non riesce, nella pagina **Riepilogo** dell'installazione guidata viene visualizzato l'errore seguente:</span><span class="sxs-lookup"><span data-stu-id="677cc-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="677cc-104">"Si è verificato un errore durante l'installazione.</span><span class="sxs-lookup"><span data-stu-id="677cc-104">"An error occurred during installation.</span></span> <span data-ttu-id="677cc-105">Il programma di installazione ha rilevato un errore che ha causato l'errore dell'installazione.</span><span class="sxs-lookup"><span data-stu-id="677cc-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="677cc-106">Contattare il produttore del software per assistenza."</span><span class="sxs-lookup"><span data-stu-id="677cc-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="677cc-107">Anche per le distribuzioni MDM, la pagina mostra un errore di installazione generico.</span><span class="sxs-lookup"><span data-stu-id="677cc-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="677cc-108">Anche se non vengono visualizzati errori esatti per gli utenti finali, microsoft mantiene un file di registro con lo stato di avanzamento dell'installazione, in **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="677cc-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="677cc-109">Ogni sessione di installazione viene aggiunta a questo file di registro.</span><span class="sxs-lookup"><span data-stu-id="677cc-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="677cc-110">Per eseguire solo l'output dell'ultima sessione di installazione, utilizzare `sed` .</span><span class="sxs-lookup"><span data-stu-id="677cc-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="677cc-111">Per altre informazioni, vedi [Risolvere i problemi di installazione per Microsoft Defender ATP per Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="677cc-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
