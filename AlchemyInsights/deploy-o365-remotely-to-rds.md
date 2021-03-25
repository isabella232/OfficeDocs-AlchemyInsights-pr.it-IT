---
title: Distribuzione di Microsoft 365 Apps for enterprise per uso condiviso in RDS, Terminal Server o VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200677"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="50ed4-102">Distribuzione di Microsoft 365 Apps for enterprise per uso condiviso in RDS, Terminal Server o VDI</span><span class="sxs-lookup"><span data-stu-id="50ed4-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="50ed4-103">Per distribuire Microsoft 365 Apps for enterprise utilizzando Servizi Desktop remoto (RDS), in precedenza denominato Servizi terminal:</span><span class="sxs-lookup"><span data-stu-id="50ed4-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="50ed4-104">È necessario disporre di un piano di Microsoft 365 For Business o di un piano di Office 365 che includa Microsoft 365 Apps for enterprise, ad esempio Office 365 Enterprise E3 o Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="50ed4-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="50ed4-105">I piani Microsoft 365 Apps for business e Microsoft 365 Business Standard non includono Microsoft 365 Apps for enterprise.</span><span class="sxs-lookup"><span data-stu-id="50ed4-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="50ed4-106">È necessario abilitare [l'attivazione di computer condivisi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="50ed4-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="50ed4-107">Puoi anche scaricare ed eseguire l'Assistente supporto e ripristino [Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) per installare Microsoft 365 Apps for enterprise in modalità di attivazione di computer condivisi.</span><span class="sxs-lookup"><span data-stu-id="50ed4-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="50ed4-108">Per ulteriori informazioni sui prerequisiti, le istruzioni di installazione e le indicazioni sulle installazioni personalizzate tramite lo Strumento di distribuzione di Office, vedere [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)</span><span class="sxs-lookup"><span data-stu-id="50ed4-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="50ed4-109">Per correggere gli errori correlati all'attivazione di computer condivisi:</span><span class="sxs-lookup"><span data-stu-id="50ed4-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="50ed4-110">Vedi [Risolvere i problemi relativi all'attivazione di computer condivisi per Microsoft 365 Apps for enterprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="50ed4-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="50ed4-111">Vedere [Reimpostare lo stato di attivazione di Microsoft 365 Apps for enterprise](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="50ed4-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="50ed4-112">Se si desidera installare Microsoft 365 Apps for enterprise in RDS dall'interfaccia di amministrazione di Microsoft 365, che utilizza le impostazioni di installazione predefinite, eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="50ed4-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="50ed4-113">Controlla quale abbonamento hai.</span><span class="sxs-lookup"><span data-stu-id="50ed4-113">Check what subscription you have.</span></span> <span data-ttu-id="50ed4-114">[Procedura](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="50ed4-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="50ed4-115">Se necessario, passare a un abbonamento diverso.</span><span class="sxs-lookup"><span data-stu-id="50ed4-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="50ed4-116">[Procedura](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="50ed4-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="50ed4-117">Se Office è già installato nel server RDS utilizzando altre sottoscrizioni Microsoft, disinstallarlo.</span><span class="sxs-lookup"><span data-stu-id="50ed4-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="50ed4-118">Ad esempio, andando a **Pannello di controllo**  >  **Disinstallare un programma**.</span><span class="sxs-lookup"><span data-stu-id="50ed4-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="50ed4-119">Disinstallare [usando Assistente supporto e ripristino Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) se si verificano problemi.</span><span class="sxs-lookup"><span data-stu-id="50ed4-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="50ed4-120">Nel server RDS, accedere all'interfaccia di amministrazione di Microsoft 365 con l'account amministratore e installare [Microsoft 365 Apps for enterprise.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="50ed4-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="50ed4-121">Dopo ***l'installazione*** di Office, non aprire o accedere ad alcuna applicazione di Office.</span><span class="sxs-lookup"><span data-stu-id="50ed4-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="50ed4-122">Nel server RDS abilitare l'attivazione di computer condivisi modificando il Registro di sistema seguendo questa procedura:</span><span class="sxs-lookup"><span data-stu-id="50ed4-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="50ed4-123">Fai clic con il pulsante destro del mouse sul pulsante Windows nell'angolo inferiore sinistro dello schermo e scegli **Esegui.**</span><span class="sxs-lookup"><span data-stu-id="50ed4-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="50ed4-124">Nella casella Apri digitare **regedit**, quindi fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="50ed4-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="50ed4-125">Selezionare **Sì** quando viene richiesto di consentire all'editor del Registro di sistema di apportare modifiche al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="50ed4-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="50ed4-126">Nell'editor del Registro di sistema aggiungi un valore stringa **SharedComputerLicensing** con un'impostazione pari a 1 in HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="50ed4-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="50ed4-127">Nel server RDS, ***accedere come*** utente finale e verificare che l'attivazione di computer condivisi sia abilitata [per Microsoft 365 Apps for enterprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="50ed4-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
