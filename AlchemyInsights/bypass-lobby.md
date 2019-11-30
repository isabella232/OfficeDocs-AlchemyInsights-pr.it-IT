---
title: Lobby di bypass
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 5ee77e57b3bc64d7a04256ab67b691e5205eac56
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626352"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Impostazioni della lobby di controllo e livello di partecipazione

Se si desidera consentire a tutti, compresi gli utenti con accesso esterno, esterni e anonimi di ignorare la lobby in Microsoft teams, è possibile utilizzare PowerShell per eseguire questa operazione. Di seguito è riportato un esempio di modifica del criterio di riunione globale per l'organizzazione:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Questo cmdlet richiede attualmente l'utilizzo del modulo di Windows PowerShell per Skype for business. Per ottenere il programma di installazione per l'utilizzo di questo cmdlet, vedere [Managing policys tramite PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

È possibile configurare un nuovo criterio, che sarà necessario applicare agli utenti. Se si modifica il criterio globale, verrà applicato automaticamente agli utenti. Per eventuali modifiche ai criteri, è necessario attendere almeno 4 ore e fino a 24 ore per rendere effettive le condizioni.

Assicurarsi di esaminare la documentazione seguente prima di apportare queste modifiche per comprendere esattamente cosa può essere consentito.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Informazioni sui controlli dei criteri di lobby riunione dei team

- [Ammetti automaticamente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) che la gente è un criterio per organizzatore che controlla se gli utenti partecipano a una riunione direttamente o attendono nella lobby finché non vengono ammessi da un utente autenticato.

- [Consenti agli utenti anonimi di avviare una riunione](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) è un criterio per ogni organizzatore che controlla se la gente anonima, inclusi i clienti B2B e federati, è in grado di partecipare alla riunione dell'utente senza un utente autenticato proveniente dall'organizzazione.

- [Consenti agli utenti con accesso esterno di ignorare la lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**prossimamente**) è un criterio per ogni organizzatore che controlla se le persone che accedono tramite telefono accedono alla riunione direttamente o attendono nella lobby, indipendentemente dall'impostazione di **ammetti persone automaticamente** .

- [Consenti agli organizzatori di ignorare le impostazioni di lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**presto disponibile**) è un criterio per ogni organizzatore che controlla se l'organizzatore della riunione può ignorare le impostazioni della lobby che un amministratore ha impostato in modo **automatico** **per consentire agli utenti di accesso esterno di ignorare la lobby** quando pianificano una nuova riunione.

**Nota:** Leggere [Manage meeting Policy in teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) per una panoramica completa dei criteri di riunione di Microsoft teams.
