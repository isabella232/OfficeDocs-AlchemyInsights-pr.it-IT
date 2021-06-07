---
title: Abilitare i webinar di Teams
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760855"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="8443b-102">Abilitare i webinar di Teams</span><span class="sxs-lookup"><span data-stu-id="8443b-102">Enable Teams Webinars</span></span>

<span data-ttu-id="8443b-103">I webinar sono abilitati per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="8443b-103">Webinars are enabled by default.</span></span> <span data-ttu-id="8443b-104">È possibile gestire chi può pianificare e registrarsi ai webinar di Teams usando i comandi Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8443b-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="8443b-105">Tutti gli utenti che possono creare una riunione possono anche creare un webinar.</span><span class="sxs-lookup"><span data-stu-id="8443b-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="8443b-106">Se si desidera gestire chi può pianificare i webinar di Teams, usare *AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="8443b-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="8443b-107">Per impostazione predefinita, *WhoCanRegister* è abilitato e impostato su **Tutti**.</span><span class="sxs-lookup"><span data-stu-id="8443b-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="8443b-108">Se si desidera disattivare la registrazione alle riunioni, impostare *AllowMeetingRegistration* su **False**.</span><span class="sxs-lookup"><span data-stu-id="8443b-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="8443b-109">Per modificare queste impostazioni, è necessario installare [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="8443b-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="8443b-110">Inoltre, i criteri riunione vengono applicati ai webinar di Teams.</span><span class="sxs-lookup"><span data-stu-id="8443b-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="8443b-111">Ad esempio, se nelle impostazioni riunione è stata disattivata la partecipazione di utenti anonimi, questi non potranno partecipare ai webinar.</span><span class="sxs-lookup"><span data-stu-id="8443b-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="8443b-112">Per altre informazioni sulla configurazione di chi può registrarsi ai webinar, vedere [Configurare chi può registrarsi ai webinar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="8443b-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="8443b-113">Per altre informazioni sulle impostazioni per Elenchi Microsoft, vedere [Controllare le impostazioni per Elenchi Microsoft](/sharepoint/control-lists).</span><span class="sxs-lookup"><span data-stu-id="8443b-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>