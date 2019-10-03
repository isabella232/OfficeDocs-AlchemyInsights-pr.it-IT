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
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="8b83b-102">Impostazioni della lobby di controllo e livello di partecipazione</span><span class="sxs-lookup"><span data-stu-id="8b83b-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="8b83b-103">Queste impostazioni controllano quali partecipanti alla riunione attendono nell'atrio prima che vengano ammessi alla riunione e il livello di partecipazione consentito in una riunione.</span><span class="sxs-lookup"><span data-stu-id="8b83b-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="8b83b-104">È possibile utilizzare PowerShell per aggiornare le impostazioni dei criteri per le riunioni che non sono state ancora implementate (contrassegnate come "prossimamente") nell'interfaccia di amministrazione dei team.</span><span class="sxs-lookup"><span data-stu-id="8b83b-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="8b83b-105">Per un esempio di cmdlet di PowerShell che consente a tutti gli utenti di ignorare la lobby, vedere di seguito.</span><span class="sxs-lookup"><span data-stu-id="8b83b-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="8b83b-106">[Ammetti automaticamente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) che la gente è un criterio per organizzatore che controlla se gli utenti partecipano a una riunione direttamente o attendono nella lobby finché non vengono ammessi da un utente autenticato.</span><span class="sxs-lookup"><span data-stu-id="8b83b-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="8b83b-107">[Consenti agli utenti anonimi di avviare una riunione](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) è un criterio per ogni organizzatore che controlla se la gente anonima, inclusi i clienti B2B e federati, è in grado di partecipare alla riunione dell'utente senza un utente autenticato proveniente dall'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="8b83b-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="8b83b-108">[Consenti agli utenti con accesso esterno di ignorare la lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**prossimamente**) è un criterio per ogni organizzatore che controlla se le persone che accedono tramite telefono accedono alla riunione direttamente o attendono nella lobby, indipendentemente dall'impostazione di **ammetti persone automaticamente** .</span><span class="sxs-lookup"><span data-stu-id="8b83b-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="8b83b-109">[Consenti agli organizzatori di ignorare le impostazioni della lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**presto disponibile**) è un criterio per ogni organizzatore che controlla se l'organizzatore della riunione può ignorare le impostazioni della lobby che un amministratore ha impostato in modo automatico per consentire agli **utenti** di accedere **in accesso esterno consente agli utenti di ignorare la lobby** quando pianificano una nuova riunione.</span><span class="sxs-lookup"><span data-stu-id="8b83b-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="8b83b-110">**Nota:** Leggere [Manage meeting Policy in teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) per una panoramica completa dei criteri di riunione di Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="8b83b-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="8b83b-111">**Esempio di PowerShell**</span><span class="sxs-lookup"><span data-stu-id="8b83b-111">**PowerShell example**</span></span>

<span data-ttu-id="8b83b-112">Se si desidera consentire a tutti, compresi gli utenti esterni o anonimi, di ignorare la lobby, è possibile utilizzare anche PowerShell per eseguire questa attività.</span><span class="sxs-lookup"><span data-stu-id="8b83b-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="8b83b-113">Di seguito è riportato un esempio di modifica del criterio di riunione globale per l'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="8b83b-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="8b83b-114">(Assicurarsi di esaminare la documentazione precedente prima di apportare queste modifiche per comprendere esattamente cosa può essere consentito).</span><span class="sxs-lookup"><span data-stu-id="8b83b-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="8b83b-115">Set-CsTeamsMeetingPolicy-Identity global-AutoAdmittedUsers "Everyone"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="8b83b-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="8b83b-116">Per ulteriori informazioni, vedere [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="8b83b-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
