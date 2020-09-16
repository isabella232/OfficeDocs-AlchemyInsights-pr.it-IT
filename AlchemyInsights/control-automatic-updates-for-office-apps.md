---
title: Controllare gli aggiornamenti automatici per le app di Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747780"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="87a1b-102">Controllare gli aggiornamenti automatici per le app di Office</span><span class="sxs-lookup"><span data-stu-id="87a1b-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="87a1b-103">Per impostazione predefinita, gli aggiornamenti per le app di Office sono scaricati automaticamente e applicati in background senza alcun intervento da parte dell'utente.</span><span class="sxs-lookup"><span data-stu-id="87a1b-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="87a1b-104">Tuttavia, gli amministratori possono controllare il modo in cui gli aggiornamenti vengono applicati usando le impostazioni di aggiornamento di Office.</span><span class="sxs-lookup"><span data-stu-id="87a1b-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="87a1b-105">Le impostazioni di aggiornamento consentono agli amministratori di abilitare o disabilitare gli aggiornamenti automatici, mostrare o nascondere il pulsante **Aggiorna adesso** in Office, impostare le scadenze degli aggiornamenti e altro ancora.</span><span class="sxs-lookup"><span data-stu-id="87a1b-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="87a1b-106">Per informazioni dettagliate, vedere:</span><span class="sxs-lookup"><span data-stu-id="87a1b-106">For detailed information, see:</span></span>

- [<span data-ttu-id="87a1b-107">Configurare le impostazioni di aggiornamento per Office</span><span class="sxs-lookup"><span data-stu-id="87a1b-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="87a1b-108">L'aggiornamento automatico per Office non è abilitato</span><span class="sxs-lookup"><span data-stu-id="87a1b-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="87a1b-109">Definire la modalità di aggiornamento di Office dopo l'installazione</span><span class="sxs-lookup"><span data-stu-id="87a1b-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="87a1b-110">Per controllare le attuali impostazioni degli aggiornamenti applicate a un computer client, eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="87a1b-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="87a1b-111">Aprire l’Editor del Registro di sistema selezionando **Avvio** > **Eseguire** > **regedit**.</span><span class="sxs-lookup"><span data-stu-id="87a1b-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="87a1b-112">Passare alla posizione seguente e rivedere le impostazioni di aggiornamento di Office:</span><span class="sxs-lookup"><span data-stu-id="87a1b-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="87a1b-113">a.</span><span class="sxs-lookup"><span data-stu-id="87a1b-113">a.</span></span> <span data-ttu-id="87a1b-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="87a1b-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="87a1b-115">b.</span><span class="sxs-lookup"><span data-stu-id="87a1b-115">b.</span></span> <span data-ttu-id="87a1b-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="87a1b-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="87a1b-117">**Nota** Se è impostata la chiave OfficeMgmtCOM, è possibile che venga visualizzato il messaggio "Gli aggiornamenti sono gestiti dall'amministratore di sistema" in **Office** > **Account** > **Aggiornamenti di Office**. </span><span class="sxs-lookup"><span data-stu-id="87a1b-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="87a1b-118">Per altre informazioni, vedere [Gestire gli aggiornamenti di Microsoft 365 Apps con Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="87a1b-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  