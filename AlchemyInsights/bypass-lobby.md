---
title: Lobby di bypass
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684954"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Impostazioni della lobby di controllo e livello di partecipazione nei team

Se si desidera consentire a tutti, compresi gli utenti con accesso esterno, esterni e anonimi, di **ignorare la lobby**, utilizzare PowerShell per eseguire questa attività. Di seguito è riportato un esempio di modifica del criterio di riunione globale per l'organizzazione.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Questo cmdlet richiede attualmente l'utilizzo del modulo di Windows PowerShell per Skype for business. Per ottenere la configurazione per l'utilizzo di questo cmdlet, vedere [Managing policys tramite PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Dopo aver configurato un criterio, è necessario applicarlo agli utenti. in alternativa, se è stato modificato il criterio globale, verrà applicato automaticamente agli utenti. Per eventuali modifiche ai criteri, è necessario attendere almeno **4 ore fino a 24 ore** per rendere effettive le condizioni. 

Assicurarsi di esaminare la documentazione seguente prima di apportare queste modifiche per comprendere esattamente cosa può essere consentito.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Informazioni sui controlli dei criteri di lobby riunione dei team

Queste impostazioni controllano quali partecipanti alla riunione attendono nell'atrio prima che vengano ammessi alla riunione e il livello di partecipazione consentito in una riunione. È possibile utilizzare PowerShell per aggiornare le impostazioni dei criteri per le riunioni che non sono state ancora implementate (contrassegnate come "prossimamente") nell'interfaccia di amministrazione dei team. Per un esempio di cmdlet di PowerShell che consente a tutti gli utenti di ignorare la lobby, vedere di seguito.

- [Ammetti automaticamente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) che la gente è un criterio per organizzatore che controlla se gli utenti partecipano a una riunione direttamente o attendono nella lobby finché non vengono ammessi da un utente autenticato.

- [Consenti agli utenti anonimi di avviare una riunione](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) è un criterio per ogni organizzatore che controlla se la gente anonima, inclusi i clienti B2B e federati, è in grado di partecipare alla riunione dell'utente senza un utente autenticato proveniente dall'organizzazione.

- [Consenti agli utenti con accesso esterno di ignorare la lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**prossimamente**) è un criterio per ogni organizzatore che controlla se le persone che accedono tramite telefono accedono alla riunione direttamente o attendono nella lobby, indipendentemente dall'impostazione di **ammetti persone automaticamente** .

- [Consenti agli organizzatori di ignorare le impostazioni di lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**presto disponibile**) è un criterio per ogni organizzatore che controlla se l'organizzatore della riunione può ignorare le impostazioni della lobby che un amministratore ha impostato in modo **automatico** **per consentire agli utenti di accesso esterno di ignorare la lobby** quando pianificano una nuova riunione.

**Nota:** Leggere [Manage meeting Policy in teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) per una panoramica completa dei criteri di riunione di Microsoft teams.
