---
title: Strumento di diagnostica dei servizi per Desktop virtuale Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590301"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="43122-102">Strumento di diagnostica dei servizi per Desktop virtuale Windows</span><span class="sxs-lookup"><span data-stu-id="43122-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="43122-103">Desktop virtuale Windows offre agli amministratori uno strumento di diagnostica per identificare gli errori tramite un'unica interfaccia.</span><span class="sxs-lookup"><span data-stu-id="43122-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="43122-104">Questo strumento registra le informazioni correlate alla diagnostica ogni volta che viene usato Desktop virtuale Windows da un utente a cui è assegnato un ruolo di Desktop virtuale Windows.</span><span class="sxs-lookup"><span data-stu-id="43122-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="43122-105">Ogni log contiene informazioni sul ruolo Desktop virtuale Windows coinvolto nell'attività, i messaggi di errore visualizzati durante la sessione e le informazioni sul tenant e l'utente.</span><span class="sxs-lookup"><span data-stu-id="43122-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="43122-106">Azure Log Analytics può essere configurato per acquisire il log attività creato dallo strumento di diagnostica tramite questa procedura:</span><span class="sxs-lookup"><span data-stu-id="43122-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="43122-107">Creare un'area di lavoro Log Analytics tramite il [portale di Azure](https://go.microsoft.com/fwlink/?linkid=2129500) o [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="43122-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="43122-108">[Connettere i computer Windows al Monitoraggio di Azure](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="43122-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="43122-109">Ottenere l'ID dell'area di lavoro e la chiave primaria dell'area di lavoro.</span><span class="sxs-lookup"><span data-stu-id="43122-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="43122-110">La configurazione della procedura guidata necessita di queste informazioni per configurare correttamente l'agente e assicurarsi che possa comunicare con il Monitoraggio di Azure.</span><span class="sxs-lookup"><span data-stu-id="43122-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="43122-111">[Eseguire il push dei dati di diagnostica nell'area di lavoro](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="43122-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="43122-112">È possibile effettuare il push dei dati di diagnostica dal tenant WVD al Log Analytics per l’area di lavoro.</span><span class="sxs-lookup"><span data-stu-id="43122-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="43122-113">[Identificare ed eseguire la diagnostica](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) dei problemi interni o esterni in relazione al Desktop virtuale Windows.</span><span class="sxs-lookup"><span data-stu-id="43122-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="43122-114">Per altre informazioni sulla configurazione dello strumento di diagnostica del servizio per Desktop virtuale Windows, vedere Uso di Log Analytics per la funzionalità di diagnostica.</span><span class="sxs-lookup"><span data-stu-id="43122-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>