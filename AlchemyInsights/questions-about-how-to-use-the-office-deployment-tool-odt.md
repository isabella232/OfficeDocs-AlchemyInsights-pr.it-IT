---
title: Domande su come usare lo Office Deployment Tool (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959687"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Domande su come usare lo Office Deployment Tool (ODT)

Scaricare lo Strumento di distribuzione di Office dall'[Area download Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Dopo il download del file, eseguire il file eseguibile autoestraente, che contiene il file eseguibile dello Strumento di distribuzione di Office (setup.exe) e un file di configurazione di esempio (configuration.xml).
  
 **Per escludere o rimuovere Microsoft 365 Apps for enterprise prodotti dai computer client:**
  
Quando si installa Microsoft 365 Apps for enterprise, è possibile escludere prodotti specifici. A questo scopo, seguire i passaggi per installare Office con lo strumento ODT, ma includere l'elemento ExcludeApp nel file di configurazione. Ad esempio, questo file di configurazione installa tutti i prodotti Microsoft 365 Apps for enterprise ad Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Panoramica dello Strumento di distribuzione di Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

