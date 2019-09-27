---
title: Installazione di Office in un server terminal-senza licenza
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205413"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="d668c-102">Installazione di Office in un server terminal</span><span class="sxs-lookup"><span data-stu-id="d668c-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="d668c-103">Per la distribuzione di Office 365 ProPlus in un server Windows utilizzando Servizi Desktop remoto (RDS), precedentemente denominato Servizi terminal:</span><span class="sxs-lookup"><span data-stu-id="d668c-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="d668c-104">È necessario disporre di un piano di Office 365 che includa Office 365 ProPlus, ad esempio Office 365 Enterprise E3 o Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="d668c-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="d668c-105">I piani di Office 365 business e Office 365 Business Premium non includono Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="d668c-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="d668c-106">È necessario abilitare l' [attivazione di computer condivisi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="d668c-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="d668c-107">Se si desidera installare Office 365 ProPlus su RDS dall'interfaccia di amministrazione di Microsoft 365, in ***cui vengono utilizzate le impostazioni di installazione predefinite***, attenersi alla seguente procedura.</span><span class="sxs-lookup"><span data-stu-id="d668c-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="d668c-108">È inoltre possibile scaricare ed eseguire l' [Assistente di supporto e ripristino Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) per installare Office 365 ProPlus in modalità di attivazione di computer condivisi.</span><span class="sxs-lookup"><span data-stu-id="d668c-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="d668c-109">Controllare il piano di Office 365.</span><span class="sxs-lookup"><span data-stu-id="d668c-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="d668c-110">Informazioni su come</span><span class="sxs-lookup"><span data-stu-id="d668c-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="d668c-111">Se necessario, passare a un altro piano di Office 365.</span><span class="sxs-lookup"><span data-stu-id="d668c-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="d668c-112">Informazioni su come</span><span class="sxs-lookup"><span data-stu-id="d668c-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="d668c-113">Se Office è già installato nel server RDS utilizzando altri piani di Office 365, disinstallarlo.</span><span class="sxs-lookup"><span data-stu-id="d668c-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="d668c-114">Ad esempio, accedendo al pannello \> di controllo, disinstallare un programma.</span><span class="sxs-lookup"><span data-stu-id="d668c-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="d668c-115">Disinstallazione tramite [Assistente di supporto e ripristino di Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se si è in esecuzione in problemi.</span><span class="sxs-lookup"><span data-stu-id="d668c-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="d668c-116">Nel server RDS accedere all'interfaccia di amministrazione di Microsoft 365 con l'account di amministratore e [installare Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="d668c-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="d668c-117">Dopo l'installazione di Office, ***non aprire o accedere*** a tutte le applicazioni di Office.</span><span class="sxs-lookup"><span data-stu-id="d668c-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="d668c-118">Nel server RDS abilitare l'attivazione di computer condivisi modificando il registro di sistema attenendosi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="d668c-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="d668c-119">Fare clic con il pulsante destro del mouse su Windows nell'angolo in basso a sinistra dello schermo e scegliere Esegui.</span><span class="sxs-lookup"><span data-stu-id="d668c-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="d668c-120">Nella casella Apri digitare **Regedit**e quindi fare clic su OK.</span><span class="sxs-lookup"><span data-stu-id="d668c-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="d668c-121">Selezionare Sì quando viene richiesto di consentire all'editor del registro di sistema di apportare modifiche al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d668c-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="d668c-122">Nell'editor del registro di sistema, aggiungere un valore stringa di **SharedComputerLicensing** con un'impostazione pari a 1 in HKEY_LOCAL_MACHINE\Software\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="d668c-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="d668c-123">Nel server RDS, ***accedere come utente finale*** e [verificare che l'attivazione di computer condivisi sia abilitata per Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="d668c-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="d668c-124">Per ulteriori informazioni sui prerequisiti, le istruzioni di installazione e le indicazioni sulle installazioni personalizzate tramite lo strumento di distribuzione di Office, vedere [deploy office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="d668c-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="d668c-125">Per correggere gli errori relativi all'attivazione di computer condivisi, vedere [risolvere i problemi relativi all'attivazione di computer condivisi per Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="d668c-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  