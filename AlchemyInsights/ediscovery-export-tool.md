---
title: Strumento di esportazione di eDiscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101306"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Non è possibile installare o eseguire lo strumento di esportazione di eDiscovery?

Se non è possibile installare o eseguire lo strumento di esportazione di eDiscovery per scaricare i risultati della ricerca, verificare quanto segue:
  
- Il computer in uso soddisfa i prerequisiti seguenti:

  - Windows 7 a 32 o 64 bit e versioni successive

  - Microsoft .NET Framework 4.7

  - Browser supportato:

  - Microsoft Edge

    Oppure

  - Internet Explorer 10 e versioni successive

    Altri browser, come Google Chrome e Mozilla Firefox, non sono supportati.

- L'organizzazione può connettersi all'endpoint in Azure, che è **\* .blob.core.windows.net** (il carattere jolly rappresenta un identificatore univoco per il processo di esportazione).

- È stato assegnato il ruolo Esporta nel Centro sicurezza Microsoft 365 &amp; sicurezza. Per impostazione predefinita, questo ruolo viene assegnato solo al gruppo di ruoli Manager eDiscovery. Vedere [Assegnare autorizzazioni di eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Per ulteriori informazioni, vedere [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Se si esportano più di 100.000 cassette postali, è necessario utilizzare powershell seguente per scaricare i risultati di esportazione: Esportazione dei risultati da più di  [100.000](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)cassette postali .