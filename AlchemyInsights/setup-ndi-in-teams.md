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
# <a name="turn-on-ndi-technology"></a>Attivare la tecnologia NDI

La tecnologia NDI richiede due passaggi per essere attivata per un utente:

1. L'amministratore tenant deve abilitare la proprietà "AllowNDIStreaming" in CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Dopo aver popolato questa modifica, l'utente finale deve attivare la tecnologia NDI® per il client specifico da Impostazioni **> autorizzazioni**.

Per ulteriori informazioni, vedere [Usare la tecnologia NDI in Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
