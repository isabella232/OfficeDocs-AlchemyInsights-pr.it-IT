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
ms.openlocfilehash: 5efb8ffad0ad2c7d32a2ac334b960484b6fa5545
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325345"
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

**Nota**: se nelle impostazioni di riunione è stata disattivata la partecipazione di utenti anonimi, tali utenti non potranno partecipare ai webinar. Per altre informazioni su come abilitare questa impostazione, vedere  [Gestire le impostazioni di riunione in Microsoft Teams](https://docs.microsoft.com/microsoftteams/meeting-settings-in-teams). 

Per altre informazioni sulla configurazione di chi può registrarsi per i webinar e su come gestire questi criteri con PowerShell di Teams, vedere [Configurare chi può registrarsi per i webinar](https://docs.microsoft.com/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Per altre informazioni sulle impostazioni per Elenchi Microsoft, vedere  [Controllare le impostazioni per Elenchi Microsoft](https://docs.microsoft.com/sharepoint/control-lists). 