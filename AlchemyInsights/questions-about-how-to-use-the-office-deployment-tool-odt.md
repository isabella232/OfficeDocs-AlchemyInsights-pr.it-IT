---
title: Domande su come utilizzare lo strumento di distribuzione di Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553544"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="420e1-102">Domande su come utilizzare lo strumento di distribuzione di Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="420e1-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="420e1-103">Scaricare lo Strumento di distribuzione di Office dall'[Area download Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="420e1-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="420e1-104">Dopo il download del file, eseguire il file eseguibile autoestraente, che contiene il file eseguibile dello Strumento di distribuzione di Office (setup.exe) e un file di configurazione di esempio (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="420e1-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="420e1-105">**Per escludere o rimuovere i prodotti di Office 365 ProPlus dai computer client:**</span><span class="sxs-lookup"><span data-stu-id="420e1-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="420e1-p101">Durante l'installazione di Office 365 ProPlus, è possibile escludere prodotti specifici. A questo scopo, seguire la procedura per l'installazione di Office con ODT, ma includere l'elemento ExcludeApp nel file di configurazione. Ad esempio, il file di configurazione installa tutti i prodotti Office 365 ProPlus ad eccezione di Publisher:</span><span class="sxs-lookup"><span data-stu-id="420e1-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="420e1-109">Panoramica dello Strumento di distribuzione di Office</span><span class="sxs-lookup"><span data-stu-id="420e1-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

