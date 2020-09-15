---
title: Strumento di esportazione di eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 55f29fae0878917eaf2972ba1dfd3c5b8a26ce54
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711099"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Non è possibile installare o eseguire lo strumento di esportazione di eDiscovery?

Se non è possibile installare o eseguire lo strumento di esportazione di eDiscovery per scaricare i risultati della ricerca, verificare le seguenti operazioni:
  
- Il computer che si sta utilizzando soddisfa questi prerequisiti:

  - Windows 7 a 32 o 64 bit e versioni successive

  - Microsoft .NET Framework 4.7

  - Browser supportato:

  - Microsoft Edge

    Oppure

  - Internet Explorer 10 e versioni successive

    Altri browser, come Google Chrome e Mozilla Firefox, non sono supportati.

- L'organizzazione può connettersi all'endpoint in Azure, che è ** \* . blob.Core.Windows.NET** (il carattere jolly rappresenta un identificatore univoco per il processo di esportazione).

- Al centro sicurezza e conformità di Microsoft 365 è assegnato il ruolo Export &amp; . Per impostazione predefinita, questo ruolo viene assegnato solo al gruppo di ruoli eDiscovery Manager. Vedere [assegnare le autorizzazioni di eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Per ulteriori informazioni, vedere [Export content search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  