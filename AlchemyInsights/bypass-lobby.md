---
title: Bypass lobby
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059600"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Controllare le impostazioni della sala di attesa e il livello di partecipazione Teams

Se si desidera consentire a tutti, inclusi gli utenti di accesso esterno, esterno e anonimo, di ignorare la **sala** di attesa, utilizzare PowerShell per eseguire questa attività. Ecco un esempio di modifica dei criteri di riunione globali per l'organizzazione.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Questo cmdlet richiede attualmente l'utilizzo di Skype for Business PowerShell. Per configurare l'utilizzo di questo cmdlet, vedere [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Dopo aver configurato un criterio, è necessario applicarlo agli utenti. oppure, se è stato modificato il criterio Globale, verrà applicato automaticamente agli utenti. Per qualsiasi modifica dei criteri, è necessario attendere almeno 4 ore fino a **24 ore** per l'applicazione dei criteri. 

Leggere la documentazione seguente prima di apportare queste modifiche per comprendere esattamente cosa consente.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Informazioni sui Teams dei criteri di sala di attesa delle riunioni

Queste impostazioni controllano quali partecipanti alla riunione devono attendere nella sala di attesa prima di essere ammessi alla riunione e il livello di partecipazione consentito in una riunione. È possibile utilizzare PowerShell per aggiornare le impostazioni dei criteri di riunione che non sono ancora state implementate (etichettate "presto") nell'interfaccia di amministrazione Teams riunione. Vedere di seguito per un esempio di cmdlet di PowerShell che consente a tutti gli utenti di ignorare la sala di attesa.

- [Ammettere automaticamente le](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) persone è un criterio per organizzatore che controlla se le persone aderiscono direttamente a una riunione o aspettano nella sala di attesa finché non vengono ammesse da un utente autenticato.

- [Consentire](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) agli utenti anonimi di avviare una riunione è un criterio per organizzatore che controlla se gli utenti anonimi, inclusi gli utenti B2B e federati, possono partecipare alla riunione dell'utente senza un utente autenticato dell'organizzazione in presenza.

- Consenti [agli](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) utenti con accesso remoto di ignorare la sala di attesa **(** presto disponibile ) è un criterio per organizzatore che controlla se le persone che aderiscono telefonicamente alla riunione direttamente o aspettano nella sala di attesa indipendentemente dall'impostazione Ammetti automaticamente le persone. 

- Consenti agli organizzatori di ignorare le impostazioni della [sala](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) di attesa **(** presto disponibile ) è un criterio per organizzatore che controlla se l'organizzatore della riunione può ignorare le impostazioni della sala di attesa impostate da un amministratore **in** Ammetti automaticamente le persone e Consenti agli utenti con accesso remoto di ignorare la **sala** di attesa quando pianificano una nuova riunione.

**Nota:** Leggere [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.
