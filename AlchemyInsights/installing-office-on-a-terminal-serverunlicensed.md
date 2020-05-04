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
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010618"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="35386-102">Installazione di Office in un server terminal</span><span class="sxs-lookup"><span data-stu-id="35386-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="35386-103">Per la distribuzione di Microsoft 365 Apps for Enterprise su un server Windows utilizzando Servizi Desktop remoto (RDS), in precedenza denominato Servizi terminal:</span><span class="sxs-lookup"><span data-stu-id="35386-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="35386-104">È necessario disporre di un abbonamento a Microsoft 365 che includa le app Microsoft 365 per Enterprise, ad esempio Office 365 Enterprise E3 o Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="35386-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="35386-105">Microsoft 365 Apps for business e Microsoft 365 Apps for Business Premium plans non include le app Microsoft 365 per Enterprise.</span><span class="sxs-lookup"><span data-stu-id="35386-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="35386-106">È necessario abilitare l' [attivazione di computer condivisi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="35386-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="35386-107">Se si desidera installare le app Microsoft 365 per Enterprise su RDS dall'interfaccia di amministrazione di Microsoft 365, in ***cui vengono utilizzate le impostazioni di installazione predefinite***, attenersi alla procedura seguente.</span><span class="sxs-lookup"><span data-stu-id="35386-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="35386-108">È inoltre possibile scaricare ed eseguire l' [Assistente di supporto e ripristino Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) per installare le app di Microsoft 365 per l'organizzazione in modalità di attivazione di computer condivisi.</span><span class="sxs-lookup"><span data-stu-id="35386-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="35386-109">Controllare la sottoscrizione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="35386-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="35386-110">Informazioni su come</span><span class="sxs-lookup"><span data-stu-id="35386-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="35386-111">Se necessario, passare a una sottoscrizione di Microsoft 365 diversa.</span><span class="sxs-lookup"><span data-stu-id="35386-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="35386-112">Informazioni su come</span><span class="sxs-lookup"><span data-stu-id="35386-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="35386-113">Se Office è già installato nel server RDS usando altre sottoscrizioni di Microsoft 365, disinstallarlo.</span><span class="sxs-lookup"><span data-stu-id="35386-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="35386-114">Ad esempio, accedendo al pannello \> di controllo, disinstallare un programma.</span><span class="sxs-lookup"><span data-stu-id="35386-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="35386-115">Disinstallazione tramite [Assistente di supporto e ripristino di Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se si è in esecuzione in problemi.</span><span class="sxs-lookup"><span data-stu-id="35386-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="35386-116">Nel server RDS accedere all'interfaccia di amministrazione di Microsoft 365 con l'account di amministratore e [installare le app di microsoft 365 per Enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="35386-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="35386-117">Dopo l'installazione di Office, ***non aprire o accedere*** a tutte le applicazioni di Office.</span><span class="sxs-lookup"><span data-stu-id="35386-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="35386-118">Nel server RDS abilitare l'attivazione di computer condivisi modificando il registro di sistema attenendosi alla procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="35386-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="35386-119">Fare clic con il pulsante destro del mouse su Windows nell'angolo in basso a sinistra dello schermo e scegliere Esegui.</span><span class="sxs-lookup"><span data-stu-id="35386-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="35386-120">Nella casella Apri digitare **Regedit**e quindi fare clic su OK.</span><span class="sxs-lookup"><span data-stu-id="35386-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="35386-121">Selezionare Sì quando viene richiesto di consentire all'editor del registro di sistema di apportare modifiche al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35386-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="35386-122">Nell'editor del registro di sistema, aggiungere un valore stringa di **SharedComputerLicensing** con un'impostazione pari a 1 in HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="35386-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="35386-123">Nel server RDS, ***accedere come utente finale*** e [verificare che l'attivazione di computer condivisi sia abilitata per le app Microsoft 365 per Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="35386-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="35386-124">Per ulteriori informazioni sui prerequisiti, le istruzioni di installazione e le indicazioni sulle installazioni personalizzate tramite lo strumento di distribuzione di Office, vedere [Deploy Microsoft 365 Apps for Enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="35386-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="35386-125">Per correggere gli errori relativi all'attivazione di computer condivisi, vedere risolvere i problemi relativi all' [attivazione di computer condivisi per le app Microsoft 365 per Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="35386-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  