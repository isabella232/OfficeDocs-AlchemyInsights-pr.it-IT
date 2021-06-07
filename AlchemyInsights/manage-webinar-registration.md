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
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783141"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="67a79-102">Gestire la registrazione ai webinar</span><span class="sxs-lookup"><span data-stu-id="67a79-102">Manage webinar registration</span></span>

<span data-ttu-id="67a79-103">È possibile gestire chi può registrarsi ai webinar di Teams usando i comandi di PowerShell per Teams.</span><span class="sxs-lookup"><span data-stu-id="67a79-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="67a79-104">Per installare PowerShell per Teams, vedere [Team PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="67a79-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="67a79-105">Per impostazione predefinita, *WhoCanRegister* è abilitato e impostato su **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="67a79-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="67a79-106">Per consentire a tutti, inclusi gli utenti anonimi, di registrarsi è necessario impostare i criteri per le riunioni su **Tutti** usando il comando di Powershell:</span><span class="sxs-lookup"><span data-stu-id="67a79-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="67a79-107">**Nota**: se nelle impostazioni di riunione è stata disattivata la partecipazione di utenti anonimi, tali utenti non potranno partecipare ai webinar.</span><span class="sxs-lookup"><span data-stu-id="67a79-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="67a79-108">Per altre informazioni e per abilitare questa impostazione, vedere [Gestire le impostazioni di riunione in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="67a79-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="67a79-109">Se si desidera disattivare la registrazione alle riunioni, impostare *AllowMeetingRegistration* su **False**.</span><span class="sxs-lookup"><span data-stu-id="67a79-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="67a79-110">Per altre informazioni sulla configurazione di chi può registrarsi ai webinar, vedere [Configurare chi può registrarsi ai webinar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="67a79-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="67a79-111">Per altre informazioni sulle impostazioni per Elenchi Microsoft, vedere [Controllare le impostazioni per Elenchi Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="67a79-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
