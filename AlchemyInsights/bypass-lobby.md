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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889086"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="877af-102">Impostazioni della lobby di controllo e livello di partecipazione nei team</span><span class="sxs-lookup"><span data-stu-id="877af-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="877af-103">Se si desidera consentire a tutti, compresi gli utenti con accesso esterno, esterni e anonimi, di **ignorare la lobby**, utilizzare PowerShell per eseguire questa attività.</span><span class="sxs-lookup"><span data-stu-id="877af-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="877af-104">Di seguito è riportato un esempio di modifica del criterio di riunione globale per l'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="877af-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="877af-105">Questo cmdlet richiede attualmente l'utilizzo del modulo di Windows PowerShell per Skype for business.</span><span class="sxs-lookup"><span data-stu-id="877af-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="877af-106">Per ottenere la configurazione per l'utilizzo di questo cmdlet, vedere [Managing policys tramite PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="877af-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="877af-107">Dopo aver configurato un criterio, è necessario applicarlo agli utenti. in alternativa, se è stato modificato il criterio globale, verrà applicato automaticamente agli utenti.</span><span class="sxs-lookup"><span data-stu-id="877af-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="877af-108">Per eventuali modifiche ai criteri, è necessario attendere almeno **4 ore fino a 24 ore** per rendere effettive le condizioni.</span><span class="sxs-lookup"><span data-stu-id="877af-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="877af-109">Assicurarsi di esaminare la documentazione seguente prima di apportare queste modifiche per comprendere esattamente cosa può essere consentito.</span><span class="sxs-lookup"><span data-stu-id="877af-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="877af-110">Informazioni sui controlli dei criteri di lobby riunione dei team</span><span class="sxs-lookup"><span data-stu-id="877af-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="877af-111">Queste impostazioni controllano quali partecipanti alla riunione attendono nell'atrio prima che vengano ammessi alla riunione e il livello di partecipazione consentito in una riunione.</span><span class="sxs-lookup"><span data-stu-id="877af-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="877af-112">È possibile utilizzare PowerShell per aggiornare le impostazioni dei criteri per le riunioni che non sono state ancora implementate (contrassegnate come "prossimamente") nell'interfaccia di amministrazione dei team.</span><span class="sxs-lookup"><span data-stu-id="877af-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="877af-113">Per un esempio di cmdlet di PowerShell che consente a tutti gli utenti di ignorare la lobby, vedere di seguito.</span><span class="sxs-lookup"><span data-stu-id="877af-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="877af-114">[Ammetti automaticamente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) che la gente è un criterio per organizzatore che controlla se gli utenti partecipano a una riunione direttamente o attendono nella lobby finché non vengono ammessi da un utente autenticato.</span><span class="sxs-lookup"><span data-stu-id="877af-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="877af-115">[Consenti agli utenti anonimi di avviare una riunione](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) è un criterio per ogni organizzatore che controlla se la gente anonima, inclusi i clienti B2B e federati, è in grado di partecipare alla riunione dell'utente senza un utente autenticato proveniente dall'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="877af-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="877af-116">[Consenti agli utenti con accesso esterno di ignorare la lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**prossimamente**) è un criterio per ogni organizzatore che controlla se le persone che accedono tramite telefono accedono alla riunione direttamente o attendono nella lobby, indipendentemente dall'impostazione di **ammetti persone automaticamente** .</span><span class="sxs-lookup"><span data-stu-id="877af-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="877af-117">[Consenti agli organizzatori di ignorare le impostazioni di lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**presto disponibile**) è un criterio per ogni organizzatore che controlla se l'organizzatore della riunione può ignorare le impostazioni della lobby che un amministratore ha impostato in modo **automatico** **per consentire agli utenti di accesso esterno di ignorare la lobby** quando pianificano una nuova riunione.</span><span class="sxs-lookup"><span data-stu-id="877af-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="877af-118">**Nota:** Leggere [Manage meeting Policy in teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) per una panoramica completa dei criteri di riunione di Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="877af-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
