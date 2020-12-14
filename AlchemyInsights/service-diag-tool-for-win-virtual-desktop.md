---
title: Strumento di diagnostica dei servizi per Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/14/2020
ms.locfileid: "49665825"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="5a6a0-102">Strumento di diagnostica dei servizi per Windows Virtual Desktop</span><span class="sxs-lookup"><span data-stu-id="5a6a0-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="5a6a0-103">Windows Virtual Desktop (WVD) offre uno strumento di diagnostica che consente agli amministratori di identificare gli errori tramite una singola interfaccia.</span><span class="sxs-lookup"><span data-stu-id="5a6a0-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="5a6a0-104">Questo strumento consente di registrare le informazioni correlate alla diagnostica ogni volta che WVD viene utilizzato da un utente assegnato a un ruolo WVD.</span><span class="sxs-lookup"><span data-stu-id="5a6a0-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="5a6a0-105">Ogni log contiene informazioni sul ruolo WVD coinvolto nell'attività, i messaggi di errore visualizzati durante la sessione e le informazioni sul tenant e sull'utente.</span><span class="sxs-lookup"><span data-stu-id="5a6a0-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="5a6a0-106">L'analisi dei log di Azure può essere configurata per acquisire il log attività creato dallo strumento di diagnostica.</span><span class="sxs-lookup"><span data-stu-id="5a6a0-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="5a6a0-107">Ecco come:</span><span class="sxs-lookup"><span data-stu-id="5a6a0-107">Here's how:</span></span>

1. <span data-ttu-id="5a6a0-108">Creare un'area di lavoro di analisi dei log con il [portale di Azure](https://go.microsoft.com/fwlink/?linkid=2129500) o [PowerShell di Azure](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="5a6a0-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="5a6a0-109">[Connettere i computer Windows a Azure monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="5a6a0-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="5a6a0-110">Ottenere l'ID dell'area di lavoro e la chiave primaria dell'area di lavoro.</span><span class="sxs-lookup"><span data-stu-id="5a6a0-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="5a6a0-111">L'installazione guidata ha bisogno di queste informazioni per configurare correttamente l'agente e per garantire che sia in grado di comunicare con Azure monitor.</span><span class="sxs-lookup"><span data-stu-id="5a6a0-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="5a6a0-112">[Inserire i dati di diagnostica nell'area di lavoro](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="5a6a0-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="5a6a0-113">È possibile inviare i dati di diagnostica dal tenant di WVD all'analisi dei log per l'area di lavoro.</span><span class="sxs-lookup"><span data-stu-id="5a6a0-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="5a6a0-114">[Identificare e diagnosticare i problemi](https://go.microsoft.com/fwlink/?linkid=2128338) interni o esterni rispetto a Wvd.</span><span class="sxs-lookup"><span data-stu-id="5a6a0-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="5a6a0-115">Per ulteriori informazioni sulla configurazione dello strumento di diagnostica dei servizi per WVD, vedere [use log Analytics for the Diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="5a6a0-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
