---
title: Strumento di esportazione di eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/3/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 5a54344d43d16c77d440768aa1c87489edf10ca0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36736329"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Non è possibile installare o eseguire lo strumento di esportazione di eDiscovery?

Se non è possibile installare o eseguire lo strumento di esportazione di Office 365 eDiscovery per scaricare i risultati della ricerca, verificare le seguenti operazioni:
  
- Il computer che si sta utilizzando soddisfa questi prerequisiti:

  - Windows 7 a 32 o 64 bit e versioni successive

  - Microsoft .NET Framework 4.7

  - Browser supportato:

  - Microsoft Edge

    Oppure

  - Internet Explorer 10 e versioni successive

    Altri browser, come Google Chrome e Mozilla Firefox, non sono supportati.

- L'organizzazione può connettersi all'endpoint in Azure, che è ** \*. blob.Core.Windows.NET** (il carattere jolly rappresenta un identificatore univoco per il processo di esportazione).

- Al centro sicurezza &amp; e conformità di Office 365 è assegnato il ruolo Export. Per impostazione predefinita, questo ruolo viene assegnato solo al gruppo di ruoli eDiscovery Manager. Vedere [assegnare le autorizzazioni di eDiscovery](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Per ulteriori informazioni, vedere [Export content search results](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  