---
title: Utilizzo dello strumento di distribuzione di Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794915"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="c81e2-102">Utilizzo dello strumento di distribuzione di Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="c81e2-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="c81e2-103">È possibile utilizzare lo strumento di distribuzione di Office per distribuire Office 365 versioni di Office.</span><span class="sxs-lookup"><span data-stu-id="c81e2-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="c81e2-104">Lo strumento di distribuzione di Office (setup.exe) viene eseguito dalla riga di comando e utilizza un file XML di configurazione per determinare le impostazioni da applicare durante la distribuzione di Office.</span><span class="sxs-lookup"><span data-stu-id="c81e2-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="c81e2-105">Scaricare la versione più recente dello strumento di distribuzione di Office dall' [area download Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="c81e2-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="c81e2-106">Utilizzare lo [strumento di personalizzazione di Office](https://config.office.com) per selezionare le preferenze di distribuzione e creare il file XML di configurazione.</span><span class="sxs-lookup"><span data-stu-id="c81e2-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="c81e2-107">Esportare il file di configurazione e posizionarlo localmente nella stessa cartella in cui risiede il setup.exe.</span><span class="sxs-lookup"><span data-stu-id="c81e2-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="c81e2-108">**Nota:** I problemi di installazione di Office si verificano generalmente a causa di file di configurazione non configurati o malformatted.</span><span class="sxs-lookup"><span data-stu-id="c81e2-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="c81e2-109">Per evitare problemi di questo tipo, è consigliabile utilizzare lo strumento di personalizzazione di Office per creare il file di configurazione.</span><span class="sxs-lookup"><span data-stu-id="c81e2-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="c81e2-110">È inoltre possibile importare i file di configurazione esistenti nello strumento di personalizzazione di Office.</span><span class="sxs-lookup"><span data-stu-id="c81e2-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="c81e2-111">Da un prompt dei comandi con privilegi elevati, passare al percorso in cui setup.exe risiede ed eseguire lo strumento di distribuzione di Office in modalità download e specificare il file di configurazione appena salvato.</span><span class="sxs-lookup"><span data-stu-id="c81e2-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="c81e2-112">In questo esempio, il file di configurazione è denominato Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="c81e2-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setup.exe /download Configuration.xml```

<span data-ttu-id="c81e2-113">4. eseguire lo strumento di distribuzione di Office in modalità configurazione e specificare il file di configurazione.</span><span class="sxs-lookup"><span data-stu-id="c81e2-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setup.exe /configure Configuration.xml```

<span data-ttu-id="c81e2-114">**Nota:** È necessario eseguire questo passaggio dal computer client in cui si desidera installare Office ed è necessario disporre delle autorizzazioni di amministratore locale su tale computer.</span><span class="sxs-lookup"><span data-stu-id="c81e2-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="c81e2-115">Per ulteriori informazioni sull'utilizzo dello strumento di distribuzione di Office per gli scenari di distribuzione di Microsoft 365 Apps for Enterprise, vedere [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="c81e2-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="c81e2-116">Per ulteriori informazioni su come utilizzare lo strumento di personalizzazione di Office, vedere [Panoramica dello strumento di personalizzazione di Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="c81e2-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
