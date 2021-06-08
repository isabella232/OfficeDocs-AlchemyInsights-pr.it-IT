---
title: Gestire la registrazione ai webinar
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798648"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="2e533-102">Gestire la registrazione ai webinar</span><span class="sxs-lookup"><span data-stu-id="2e533-102">Manage webinar registration</span></span>

<span data-ttu-id="2e533-103">È possibile gestire chi può registrarsi ai webinar di Teams usando i comandi di PowerShell per Teams.</span><span class="sxs-lookup"><span data-stu-id="2e533-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="2e533-104">Per installare PowerShell per Teams, vedere [Team PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="2e533-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="2e533-105">Per impostazione predefinita, *WhoCanRegister* è abilitato e impostato su **Tutti**.</span><span class="sxs-lookup"><span data-stu-id="2e533-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="2e533-106">Se non viene visualizzata l'opzione per consentire la registrazione a Tutti nell'invito della riunione, impostare di nuovo *WhoCanRegister* su Tutti e attendere 24 ore.</span><span class="sxs-lookup"><span data-stu-id="2e533-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="2e533-107">Per eseguire di nuovo *WhoCanRegister*, usare il comando Powershell:</span><span class="sxs-lookup"><span data-stu-id="2e533-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="2e533-108">**Nota**: se nelle impostazioni di riunione è stata disattivata la partecipazione di utenti anonimi, tali utenti non potranno partecipare ai webinar.</span><span class="sxs-lookup"><span data-stu-id="2e533-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="2e533-109">Per altre informazioni e per abilitare questa impostazione, vedere [Gestire le impostazioni di riunione in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="2e533-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="2e533-110">Se si desidera disattivare la registrazione alle riunioni, impostare *AllowMeetingRegistration* su **False**.</span><span class="sxs-lookup"><span data-stu-id="2e533-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="2e533-111">Per altre informazioni sulla configurazione di chi può registrarsi ai webinar, vedere [Configurare chi può registrarsi ai webinar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="2e533-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="2e533-112">Per altre informazioni sulle impostazioni per Elenchi Microsoft, vedere [Controllare le impostazioni per Elenchi Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="2e533-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
