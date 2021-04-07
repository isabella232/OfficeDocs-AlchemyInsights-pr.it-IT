---
title: Identificare i problemi del Desktop virtuale Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590296"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="2f5a3-102">Identificare i problemi del Desktop virtuale Windows</span><span class="sxs-lookup"><span data-stu-id="2f5a3-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="2f5a3-103">La diagnostica del Desktop virtuale di Windows usa un solo cmdlet di PowerShell ma contiene diversi parametri facoltativi che consentono di restringere e isolare i problemi.</span><span class="sxs-lookup"><span data-stu-id="2f5a3-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="2f5a3-104">Per iniziare:</span><span class="sxs-lookup"><span data-stu-id="2f5a3-104">To get started:</span></span> 

1. <span data-ttu-id="2f5a3-105">Scaricare e importare il modulo PowerShell per il Desktop virtuale Windows.</span><span class="sxs-lookup"><span data-stu-id="2f5a3-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="2f5a3-106">Per informazioni dettagliate, vedere [Cmdlet del Desktop virtuale Windows per Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span><span class="sxs-lookup"><span data-stu-id="2f5a3-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="2f5a3-107">Eseguire il cmdlet seguente per accedere al proprio account:</span><span class="sxs-lookup"><span data-stu-id="2f5a3-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="2f5a3-108">Esempio: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="2f5a3-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="2f5a3-109">**NOTA:** tutte le query che usano PowerShell devono includere il parametro -UserName o -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="2f5a3-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="2f5a3-110">Per le funzionalità di monitoraggio, vedere [Uso di Log Analytics per la funzionalità di diagnostica](https://go.microsoft.com/fwlink/?linkid=2126847).</span><span class="sxs-lookup"><span data-stu-id="2f5a3-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="2f5a3-111">Per filtrare le attività di diagnostica per utente, eseguire il cmdlet seguente:</span><span class="sxs-lookup"><span data-stu-id="2f5a3-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="2f5a3-112">Esempio: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="2f5a3-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="2f5a3-113">È disponibile un elenco di filtri che è possibile eseguire per la diagnosi dei problemi.</span><span class="sxs-lookup"><span data-stu-id="2f5a3-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="2f5a3-114">Per altre informazioni sulla diagnostica dei problemi, vedere[Identificare e diagnosticare i problemi del Desktop virtuale Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="2f5a3-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="2f5a3-115">Per altre informazioni sugli errori comuni, vedere [Scenari di errori comuni](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="2f5a3-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
