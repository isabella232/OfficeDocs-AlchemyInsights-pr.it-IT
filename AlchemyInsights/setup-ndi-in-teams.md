---
title: Attivare la tecnologia NDI
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/21/2021
ms.locfileid: "49917314"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="8ca18-102">Attivare la tecnologia NDI</span><span class="sxs-lookup"><span data-stu-id="8ca18-102">Turn on NDI technology</span></span>

<span data-ttu-id="8ca18-103">La tecnologia NDI richiede due passaggi per essere attivata per un utente:</span><span class="sxs-lookup"><span data-stu-id="8ca18-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="8ca18-104">L'amministratore tenant deve abilitare la proprietà "AllowNDIStreaming" in CsTeamsMeetingPolicy.</span><span class="sxs-lookup"><span data-stu-id="8ca18-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="8ca18-105">Dopo aver popolato questa modifica, l'utente finale deve attivare la tecnologia NDI® per il client specifico da Impostazioni **> autorizzazioni**.</span><span class="sxs-lookup"><span data-stu-id="8ca18-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="8ca18-106">Per ulteriori informazioni, vedere [Usare la tecnologia NDI in Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)</span><span class="sxs-lookup"><span data-stu-id="8ca18-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
