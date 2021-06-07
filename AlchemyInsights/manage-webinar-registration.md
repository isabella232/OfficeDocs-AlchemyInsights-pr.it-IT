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
# <a name="manage-webinar-registration"></a>Gestire la registrazione ai webinar

È possibile gestire chi può registrarsi ai webinar di Teams usando i comandi Teams PowerShell. Per impostazione predefinita, *WhoCanRegister* è abilitato e impostato su **Tutti**. Se si desidera disattivare la registrazione alle riunioni, impostare *AllowMeetingRegistration* su **False**.

Per modificare queste impostazioni, è necessario installare [Teams PowerShell](/microsoftteams/teams-powershell-install). Inoltre, i criteri riunione vengono applicati ai webinar di Teams. Ad esempio, se nelle impostazioni riunione è stata disattivata la partecipazione di utenti anonimi, questi non potranno partecipare ai webinar.

Per altre informazioni sulla configurazione di chi può registrarsi ai webinar, vedere [Configurare chi può registrarsi ai webinar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Per altre informazioni sulle impostazioni per Elenchi Microsoft, vedere [Controllare le impostazioni per Elenchi Microsoft](/sharepoint/control-lists).