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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376705"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Impostazioni della lobby di controllo e livello di partecipazione

Queste impostazioni controllano quali partecipanti alla riunione attendono nell'atrio prima che vengano ammessi alla riunione e il livello di partecipazione consentito in una riunione. È possibile utilizzare PowerShell per aggiornare le impostazioni dei criteri per le riunioni che non sono state ancora implementate (contrassegnate come "prossimamente") nell'interfaccia di amministrazione dei team.  Per un esempio di cmdlet di PowerShell che consente a tutti gli utenti di ignorare la lobby, vedere di seguito.  

- [Ammetti automaticamente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) che la gente è un criterio per organizzatore che controlla se gli utenti partecipano a una riunione direttamente o attendono nella lobby finché non vengono ammessi da un utente autenticato.

- [Consenti agli utenti anonimi di avviare una riunione](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) è un criterio per ogni organizzatore che controlla se la gente anonima, inclusi i clienti B2B e federati, è in grado di partecipare alla riunione dell'utente senza un utente autenticato proveniente dall'organizzazione.

- [Consenti agli utenti con accesso esterno di ignorare la lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**prossimamente**) è un criterio per ogni organizzatore che controlla se le persone che accedono tramite telefono accedono alla riunione direttamente o attendono nella lobby, indipendentemente dall'impostazione di **ammetti persone automaticamente** .

- [Consenti agli organizzatori di ignorare le impostazioni della lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**presto disponibile**) è un criterio per ogni organizzatore che controlla se l'organizzatore della riunione può ignorare le impostazioni della lobby che un amministratore ha impostato in modo automatico per consentire agli **utenti** di accedere **in accesso esterno consente agli utenti di ignorare la lobby** quando pianificano una nuova riunione.

**Nota:** Leggere [Manage meeting Policy in teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) per una panoramica completa dei criteri di riunione di Microsoft teams. 


**Esempio di PowerShell**

Se si desidera consentire a tutti, compresi gli utenti esterni o anonimi, di ignorare la lobby, è possibile utilizzare anche PowerShell per eseguire questa attività.  Di seguito è riportato un esempio di modifica del criterio di riunione globale per l'organizzazione.   

(Assicurarsi di esaminare la documentazione precedente prima di apportare queste modifiche per comprendere esattamente cosa può essere consentito).

Set-CsTeamsMeetingPolicy-Identity global-AutoAdmittedUsers "Everyone"-AllowPSTNUsersToBypassLobby $True

Per ulteriori informazioni, vedere [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
