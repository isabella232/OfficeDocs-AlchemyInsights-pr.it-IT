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
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820038"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="8a9e3-102">Controllare le impostazioni della sala di attesa e il livello di partecipazione in Teams</span><span class="sxs-lookup"><span data-stu-id="8a9e3-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="8a9e3-103">Se si desidera consentire a tutti, inclusi gli utenti di accesso esterno, esterno e anonimo, di ignorare la **sala** di attesa, utilizzare PowerShell per eseguire questa attività.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="8a9e3-104">Ecco un esempio di modifica dei criteri di riunione globali per l'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="8a9e3-105">Questo cmdlet richiede attualmente l'uso del modulo di PowerShell di Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="8a9e3-106">Per configurare l'utilizzo di questo cmdlet, vedere [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="8a9e3-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="8a9e3-107">Dopo aver configurato un criterio, è necessario applicarlo agli utenti. oppure, se è stato modificato il criterio Globale, verrà applicato automaticamente agli utenti.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="8a9e3-108">Per qualsiasi modifica dei criteri, è necessario attendere almeno 4 ore fino a **24 ore** per l'applicazione dei criteri.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="8a9e3-109">Leggere la documentazione seguente prima di apportare queste modifiche per comprendere esattamente cosa consente.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="8a9e3-110">Informazioni sui controlli dei criteri di sala di attesa per le riunioni di Teams</span><span class="sxs-lookup"><span data-stu-id="8a9e3-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="8a9e3-111">Queste impostazioni controllano quali partecipanti alla riunione devono attendere nella sala di attesa prima di essere ammessi alla riunione e il livello di partecipazione consentito in una riunione.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="8a9e3-112">È possibile utilizzare PowerShell per aggiornare le impostazioni dei criteri riunione che non sono ancora state implementate (etichettate "presto") nell'interfaccia di amministrazione di Teams.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="8a9e3-113">Vedere di seguito per un esempio di cmdlet di PowerShell che consente a tutti gli utenti di ignorare la sala di attesa.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="8a9e3-114">[Ammettere automaticamente le](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) persone è un criterio per organizzatore che controlla se le persone aderiscono direttamente a una riunione o aspettano nella sala di attesa finché non vengono ammesse da un utente autenticato.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="8a9e3-115">[Consentire](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) agli utenti anonimi di avviare una riunione è un criterio per organizzatore che controlla se gli utenti anonimi, inclusi gli utenti B2B e federati, possono partecipare alla riunione dell'utente senza un utente autenticato dell'organizzazione in presenza.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="8a9e3-116">Consenti [agli](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) utenti con accesso remoto di ignorare la sala di attesa **(** presto disponibile ) è un criterio per organizzatore che controlla se le persone che aderiscono telefonicamente alla riunione direttamente o aspettano nella sala di attesa indipendentemente dall'impostazione Ammetti automaticamente le persone. </span><span class="sxs-lookup"><span data-stu-id="8a9e3-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="8a9e3-117">Consenti agli organizzatori di ignorare le impostazioni della [sala](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) di attesa **(** presto disponibile ) è un criterio per organizzatore che controlla se l'organizzatore della riunione può ignorare le impostazioni della sala di attesa impostate da un amministratore **in** Ammetti automaticamente le persone e Consenti agli utenti con accesso remoto di ignorare la **sala** di attesa quando pianificano una nuova riunione.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="8a9e3-118">**Nota:** Leggere [Gestire i criteri riunione in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) per una panoramica completa dei criteri di riunione di Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8a9e3-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
