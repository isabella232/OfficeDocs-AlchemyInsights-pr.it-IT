---
title: Domande su come utilizzare lo strumento di distribuzione di Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698062"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="a2117-102">Domande su come utilizzare lo strumento di distribuzione di Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="a2117-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="a2117-103">Scaricare lo Strumento di distribuzione di Office dall'[Area download Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="a2117-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="a2117-104">Dopo il download del file, eseguire il file eseguibile autoestraente, che contiene il file eseguibile dello Strumento di distribuzione di Office (setup.exe) e un file di configurazione di esempio (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="a2117-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="a2117-105">**Per escludere o rimuovere le app Microsoft 365 per i prodotti Enterprise dai computer client:**</span><span class="sxs-lookup"><span data-stu-id="a2117-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="a2117-106">Quando si installano le app di Microsoft 365 per Enterprise, è possibile escludere prodotti specifici.</span><span class="sxs-lookup"><span data-stu-id="a2117-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="a2117-107">A questo scopo, seguire i passaggi per installare Office con lo strumento ODT, ma includere l'elemento ExcludeApp nel file di configurazione.</span><span class="sxs-lookup"><span data-stu-id="a2117-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="a2117-108">Ad esempio, questo file di configurazione consente di installare tutte le app Microsoft 365 per i prodotti Enterprise ad eccezione di Publisher:</span><span class="sxs-lookup"><span data-stu-id="a2117-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="a2117-109">Panoramica dello Strumento di distribuzione di Office</span><span class="sxs-lookup"><span data-stu-id="a2117-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

