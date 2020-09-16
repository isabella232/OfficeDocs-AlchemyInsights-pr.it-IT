---
title: Cambiare i canali di aggiornamento per le app di Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 70b416e2b572fe9b4257648e3426b4d36975681e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756503"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="8f366-102">Cambiare i canali di aggiornamento per le app di Office</span><span class="sxs-lookup"><span data-stu-id="8f366-102">Change update channels for Office apps</span></span>

<span data-ttu-id="8f366-103">Per le nuove installazioni di Office, usare le impostazioni di download del software Office per selezionare il canale di aggiornamento desiderato, quindi installare o reinstallare le app di Office.</span><span class="sxs-lookup"><span data-stu-id="8f366-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="8f366-104">Per altre informazioni, si veda [Gestire le impostazioni di download del software in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span><span class="sxs-lookup"><span data-stu-id="8f366-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="8f366-105">**Nota** Il canale di aggiornamento selezionato con le impostazioni di download del software Office si applica a tutti gli utenti che eseguono nuove installazioni usando il portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f366-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="8f366-106">Per altre informazioni, si veda [Scaricare e installare o reinstallare Microsoft 365 o Office 2019 in un PC o Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span><span class="sxs-lookup"><span data-stu-id="8f366-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="8f366-107">Per le installazioni di Office esistenti, usare lo strumento di distribuzione di Office (ODT) per passare a un altro canale di aggiornamento:</span><span class="sxs-lookup"><span data-stu-id="8f366-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="8f366-108">Scaricare la versione più recente dello strumento di distribuzione di Office (setup.exe) dall'[Area download Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="8f366-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="8f366-109">Identificare il nome del canale a cui si vuole passare.</span><span class="sxs-lookup"><span data-stu-id="8f366-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="8f366-110">Per altre informazioni, vedere [Opzioni di configurazione per lo strumento di distribuzione di Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span><span class="sxs-lookup"><span data-stu-id="8f366-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="8f366-111">Creare un file XML di configurazione specificando il nome del canale appropriato, ad esempio update.xml.</span><span class="sxs-lookup"><span data-stu-id="8f366-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  

`<Configuration>`<br>
`<Updates Channel="Current"/>`<br>
`</Configuration>`<br>

4. <span data-ttu-id="8f366-112">Da un prompt dei comandi con privilegi elevati, passare alla posizione della cartella in cui risiede il file setup.exe ed eseguire il comando seguente:</span><span class="sxs-lookup"><span data-stu-id="8f366-112">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="8f366-113">a.</span><span class="sxs-lookup"><span data-stu-id="8f366-113">a.</span></span> <span data-ttu-id="8f366-114">setup.exe /configura update.xml</span><span class="sxs-lookup"><span data-stu-id="8f366-114">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="8f366-115">Avviare un'applicazione di Office, ad esempio Excel, quindi selezionare **File** > **Account**.</span><span class="sxs-lookup"><span data-stu-id="8f366-115">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="8f366-116">Nella sezione Informazioni sul prodotto selezionare **Opzioni di aggiornamento** > **Aggiorna ora**.</span><span class="sxs-lookup"><span data-stu-id="8f366-116">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="8f366-117">Per altre informazioni, si veda [Come cambiare canale di aggiornamento per le app di Office esistenti](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span><span class="sxs-lookup"><span data-stu-id="8f366-117">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="8f366-118">Per cambiare canale di aggiornamento per un gruppo selezionato di utenti o con Configuration Manager (SCCM), configurare l'impostazione del canale di aggiornamento tramite oggetto Criteri di gruppo.</span><span class="sxs-lookup"><span data-stu-id="8f366-118">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="8f366-119">Per altre informazioni, vedere [Panoramica dei canali di aggiornamento per Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span><span class="sxs-lookup"><span data-stu-id="8f366-119">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="8f366-120">Per informazioni dettagliate, vedere [Come gestire i canali di Office 365 ProPlus per i professionisti IT](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) e [Gestire gli aggiornamenti alle app di Microsoft 365 con Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="8f366-120">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>