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
# <a name="manage-webinar-registration"></a>Gestire la registrazione ai webinar

È possibile gestire chi può registrarsi ai webinar di Teams usando i comandi di PowerShell per Teams. Per installare PowerShell per Teams, vedere [Team PowerShell](/microsoftteams/teams-powershell-install). 

Per impostazione predefinita, *WhoCanRegister* è abilitato e impostato su **EveryoneInCompany**. Per consentire a tutti, inclusi gli utenti anonimi, di registrarsi è necessario impostare i criteri per le riunioni su **Tutti** usando il comando di Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Nota**: se nelle impostazioni di riunione è stata disattivata la partecipazione di utenti anonimi, tali utenti non potranno partecipare ai webinar. Per altre informazioni e per abilitare questa impostazione, vedere [Gestire le impostazioni di riunione in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Se si desidera disattivare la registrazione alle riunioni, impostare *AllowMeetingRegistration* su **False**.

Per altre informazioni sulla configurazione di chi può registrarsi ai webinar, vedere [Configurare chi può registrarsi ai webinar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Per altre informazioni sulle impostazioni per Elenchi Microsoft, vedere [Controllare le impostazioni per Elenchi Microsoft](/sharepoint/control-lists).
