---
title: Domande sull'utilizzo di Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28295761"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Domande sull'utilizzo di Office Deployment Tool (ODT)

Scaricare lo Strumento di distribuzione di Office dall'[Area download Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Dopo il download del file, eseguire il file eseguibile autoestraente, che contiene il file eseguibile dello Strumento di distribuzione di Office (setup.exe) e un file di configurazione di esempio (configuration.xml).
  
 **Per escludere o rimuovere prodotti Office 365 ProPlus dal computer client:**
  
Durante l'installazione di Office 365 ProPlus, è possibile escludere prodotti specifici. A questo scopo, seguire la procedura per l'installazione di Office con ODT, ma includere l'elemento ExcludeApp nel file di configurazione. Ad esempio, il file di configurazione installa tutti i prodotti Office 365 ProPlus ad eccezione di Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Panoramica dello Strumento di distribuzione di Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

