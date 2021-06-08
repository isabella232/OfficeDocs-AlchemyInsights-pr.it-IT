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
# <a name="manage-webinar-registration"></a>Gestire la registrazione ai webinar

È possibile gestire chi può registrarsi ai webinar di Teams usando i comandi di PowerShell per Teams. Per installare PowerShell per Teams, vedere [Team PowerShell](/microsoftteams/teams-powershell-install). 

Per impostazione predefinita, *WhoCanRegister* è abilitato e impostato su **Tutti**. 

Se non viene visualizzata l'opzione per consentire la registrazione a Tutti nell'invito della riunione, impostare di nuovo *WhoCanRegister* su Tutti e attendere 24 ore. Per eseguire di nuovo *WhoCanRegister*, usare il comando Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Nota**: se nelle impostazioni di riunione è stata disattivata la partecipazione di utenti anonimi, tali utenti non potranno partecipare ai webinar. Per altre informazioni e per abilitare questa impostazione, vedere [Gestire le impostazioni di riunione in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Se si desidera disattivare la registrazione alle riunioni, impostare *AllowMeetingRegistration* su **False**.

Per altre informazioni sulla configurazione di chi può registrarsi ai webinar, vedere [Configurare chi può registrarsi ai webinar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Per altre informazioni sulle impostazioni per Elenchi Microsoft, vedere [Controllare le impostazioni per Elenchi Microsoft](/sharepoint/control-lists).
