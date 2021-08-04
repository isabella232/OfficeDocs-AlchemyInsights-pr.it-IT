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
ms.openlocfilehash: a56abdaae182b840a1a96466e0581ef49b2b0075
ms.sourcegitcommit: 540a4e2515f7cfddee65519046454fc4437cd287
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/01/2021
ms.locfileid: "53688978"
---
# <a name="enable-teams-webinars"></a>Abilitare i webinar di Teams

La registrazione al webinar è attivata per impostazione predefinita. Se si vuole disattivare la registrazione alla riunione, è possibile usare l'interfaccia di amministrazione di Teams: 

1. Passare all'[interfaccia di amministrazione di Teams](https://admin.teams.microsoft.com/policies/meetings). 

2. Selezionare il criterio **Globale (predefinito a livello di organizzazione)** o altri criteri specifici. 

3. In **Generale**, impostare **Consenti registrazione riunione** su **Disattivato**. 

Quando la registrazione alla riunione è impostata su **Attivato**, è anche possibile gestire chi si registra per i webinar di Teams usando l'interfaccia di amministrazione di Teams: 

1. Passare all'[interfaccia di amministrazione di Teams](https://admin.teams.microsoft.com/policies/meetings). 

2. Selezionare il criterio **Globale (predefinito a livello di organizzazione)** o altri criteri specifici. 

3. In **Generale**, passare all'impostazione **Chi può registrare** e selezionare **Tutti** o **Tutti nell’azienda**. 

**Nota**: se nelle impostazioni di riunione è stata disattivata la partecipazione di utenti anonimi, tali utenti non potranno partecipare ai webinar. Per altre informazioni su come abilitare questa impostazione, vedere  [Gestire le impostazioni di riunione in Microsoft Teams](/microsoftteams/meeting-settings-in-teams). 

Per altre informazioni sulla configurazione di chi può registrarsi per i webinar e su come gestire questi criteri con PowerShell di Teams, vedere [Configurare chi può registrarsi per i webinar](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Per altre informazioni sulle impostazioni per Elenchi Microsoft, vedere  [Controllare le impostazioni per Elenchi Microsoft](/sharepoint/control-lists). 