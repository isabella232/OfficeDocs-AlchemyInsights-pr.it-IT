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
ms.openlocfilehash: 988e97896cc1000c11ce1e81cd169090b1c39104
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760847"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="07f00-102">Gestire la registrazione ai webinar</span><span class="sxs-lookup"><span data-stu-id="07f00-102">Manage webinar registration</span></span>

<span data-ttu-id="07f00-103">È possibile gestire chi può registrarsi ai webinar di Teams usando i comandi Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="07f00-103">You can manage who can register for Teams Webinars by using Teams PowerShell commands.</span></span> <span data-ttu-id="07f00-104">Per impostazione predefinita, *WhoCanRegister* è abilitato e impostato su **Tutti**.</span><span class="sxs-lookup"><span data-stu-id="07f00-104">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="07f00-105">Se si desidera disattivare la registrazione alle riunioni, impostare *AllowMeetingRegistration* su **False**.</span><span class="sxs-lookup"><span data-stu-id="07f00-105">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="07f00-106">Per modificare queste impostazioni, è necessario installare [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="07f00-106">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="07f00-107">Inoltre, i criteri riunione vengono applicati ai webinar di Teams.</span><span class="sxs-lookup"><span data-stu-id="07f00-107">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="07f00-108">Ad esempio, se nelle impostazioni riunione è stata disattivata la partecipazione di utenti anonimi, questi non potranno partecipare ai webinar.</span><span class="sxs-lookup"><span data-stu-id="07f00-108">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="07f00-109">Per altre informazioni sulla configurazione di chi può registrarsi ai webinar, vedere [Configurare chi può registrarsi ai webinar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="07f00-109">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="07f00-110">Per altre informazioni sulle impostazioni per Elenchi Microsoft, vedere [Controllare le impostazioni per Elenchi Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="07f00-110">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>