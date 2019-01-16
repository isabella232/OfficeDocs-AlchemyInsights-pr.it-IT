---
title: Utilizzo dello strumento di distribuzione di Office
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296606"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="dae5d-102">Using the Office Deployment Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="dae5d-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="dae5d-p101">Utilizzare Office Deployment Tool (ODT) per distribuire Office 365 le versioni di Office. Lo strumento di distribuzione di Office (setup.exe) eseguire dalla riga di comando e viene utilizzato un file XML di configurazione per determinare le impostazioni da applicare durante la distribuzione di Office.</span><span class="sxs-lookup"><span data-stu-id="dae5d-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="dae5d-105">Scaricare la versione più recente di Office Deployment Tool dall' [Area Download Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="dae5d-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="dae5d-p102">Utilizzare [Office Customization Tool (OCT)](https://config.office.com) per selezionare le preferenze di distribuzione e creare file di configurazione XML. Esportare il file di configurazione e inserirli localmente nella stessa cartella in cui risiede il setup.exe.</span><span class="sxs-lookup"><span data-stu-id="dae5d-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="dae5d-p103">**Nota:** Installazione di Office in genere si verificano problemi dovuti a non correttamente configurato o i file di configurazione valido. Per evitare tali problemi, è consigliabile utilizzare lo strumento di personalizzazione di Office per creare il file di configurazione. È inoltre possibile importare file di configurazione esistenti nello strumento di personalizzazione di Office.</span><span class="sxs-lookup"><span data-stu-id="dae5d-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="dae5d-p104">Da un prompt dei comandi con privilegi elevati, passare alla posizione in cui risiede setup.exe eseguire lo strumento di distribuzione di Office in modalità download e specificare il file di configurazione che appena salvato. In questo esempio il file di configurazione denominato Configuration. XML:</span><span class="sxs-lookup"><span data-stu-id="dae5d-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="dae5d-113">Eseguire lo strumento di distribuzione di Office in modalità configure e specificare il file di configurazione.</span><span class="sxs-lookup"><span data-stu-id="dae5d-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="dae5d-114">**Nota:** È necessario eseguire questo passaggio dal computer client in cui si desidera installare Office, quindi è necessario disporre delle autorizzazioni di amministratore locale nel computer.</span><span class="sxs-lookup"><span data-stu-id="dae5d-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="dae5d-p105">Per ulteriori informazioni sull'utilizzo dello strumento di distribuzione di Office per gli scenari di distribuzione di Office 365 ProPlus, vedere [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). Per ulteriori informazioni su come utilizzare lo strumento di personalizzazione di Office, vedere [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="dae5d-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

