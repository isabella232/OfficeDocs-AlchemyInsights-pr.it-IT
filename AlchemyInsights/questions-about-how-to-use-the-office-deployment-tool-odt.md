---
title: Domande su come utilizzare lo strumento di distribuzione di Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086160"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Domande su come utilizzare lo strumento di distribuzione di Office (ODT)

Scaricare lo Strumento di distribuzione di Office dall'[Area download Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Dopo il download del file, eseguire il file eseguibile autoestraente, che contiene l'eseguibile dello strumento di distribuzione di Office (setupodt.exe) e un file di configurazione di esempio (configuration.xml).
  
 **Per escludere o rimuovere le app Microsoft 365 per i prodotti Enterprise dai computer client:**
  
Quando si installano le app di Microsoft 365 per Enterprise, è possibile escludere prodotti specifici. A questo scopo, seguire i passaggi per installare Office con lo strumento ODT, ma includere l'elemento ExcludeApp nel file di configurazione. Ad esempio, questo file di configurazione consente di installare tutte le app Microsoft 365 per i prodotti Enterprise ad eccezione di Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Panoramica dello Strumento di distribuzione di Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

