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
ms.openlocfilehash: d6ffd69cdc02331ecd1290fa3b0cb5a542c8bd58
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528267"
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

- Al centro sicurezza &amp; e conformità di Office 365 è assegnato il ruolo Export. Per impostazione predefinita, questo ruolo viene assegnato solo al gruppo di ruoli eDiscovery Manager. Vedere [assegnare le autorizzazioni di eDiscovery](https://support.office.com/article/assign-ediscovery-permissions-in-the-office-365-security-compliance-center-5b9a067b-9d2e-4aa5-bb33-99d8c0d0b5d7#moreinfo).

Per ulteriori informazioni, vedere [Export content search results](https://support.office.com/article/Export-Content-Search-results-from-the-Office-365-Security-Compliance-Center-ed48d448-3714-4c42-85f5-10f75f6a4278).
  