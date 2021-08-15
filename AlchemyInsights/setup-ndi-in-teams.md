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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023526"
---
# <a name="turn-on-ndi-technology"></a>Attivare la tecnologia NDI

La tecnologia NDI richiede due passaggi per essere attivata per un utente:

1. L'amministratore tenant deve abilitare la proprietà 'AllowNDIStreaming' in CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Dopo aver popolato questa modifica, l'utente finale deve attivare la tecnologia NDI® per il proprio client specifico da **Impostazioni > Autorizzazioni**.

Per ulteriori informazioni, vedere [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
