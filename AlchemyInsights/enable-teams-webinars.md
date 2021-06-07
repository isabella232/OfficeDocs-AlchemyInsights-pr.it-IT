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
# <a name="enable-teams-webinars"></a>Abilitare i webinar di Teams

I webinar sono abilitati per impostazione predefinita. È possibile gestire chi può pianificare e registrarsi ai webinar di Teams usando i comandi Teams PowerShell.

- Tutti gli utenti che possono creare una riunione possono anche creare un webinar. Se si desidera gestire chi può pianificare i webinar di Teams, usare *AllowMeetingRegistration*. 
- Per impostazione predefinita, *WhoCanRegister* è abilitato e impostato su **Tutti**. Se si desidera disattivare la registrazione alle riunioni, impostare *AllowMeetingRegistration* su **False**.

Per modificare queste impostazioni, è necessario installare [Teams PowerShell](/microsoftteams/teams-powershell-install). Inoltre, i criteri riunione vengono applicati ai webinar di Teams. Ad esempio, se nelle impostazioni riunione è stata disattivata la partecipazione di utenti anonimi, questi non potranno partecipare ai webinar.

Per altre informazioni sulla configurazione di chi può registrarsi ai webinar, vedere [Configurare chi può registrarsi ai webinar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Per altre informazioni sulle impostazioni per Elenchi Microsoft, vedere [Controllare le impostazioni per Elenchi Microsoft](/sharepoint/control-lists).