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
# <a name="identify-windows-virtual-desktop-issues"></a>Identificare i problemi del Desktop virtuale Windows

La diagnostica del Desktop virtuale di Windows usa un solo cmdlet di PowerShell ma contiene diversi parametri facoltativi che consentono di restringere e isolare i problemi. Per iniziare: 

1. Scaricare e importare il modulo PowerShell per il Desktop virtuale Windows. Per informazioni dettagliate, vedere [Cmdlet del Desktop virtuale Windows per Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. Eseguire il cmdlet seguente per accedere al proprio account:
    
    Esempio: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**NOTA:** tutte le query che usano PowerShell devono includere il parametro -UserName o -ActivityID. Per le funzionalità di monitoraggio, vedere [Uso di Log Analytics per la funzionalità di diagnostica](https://go.microsoft.com/fwlink/?linkid=2126847).

Per filtrare le attività di diagnostica per utente, eseguire il cmdlet seguente:

Esempio: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

È disponibile un elenco di filtri che è possibile eseguire per la diagnosi dei problemi. Per altre informazioni sulla diagnostica dei problemi, vedere[Identificare e diagnosticare i problemi del Desktop virtuale Windows](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

Per altre informazioni sugli errori comuni, vedere [Scenari di errori comuni](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
