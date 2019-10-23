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
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637781"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="a6225-102">Impostazioni della lobby di controllo e livello di partecipazione</span><span class="sxs-lookup"><span data-stu-id="a6225-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="a6225-103">Se si desidera consentire a tutti, compresi gli utenti con accesso esterno, esterni e anonimi, di ignorare la lobby, è possibile utilizzare PowerShell per eseguire questa operazione.</span><span class="sxs-lookup"><span data-stu-id="a6225-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="a6225-104">Di seguito è riportato un esempio di modifica del criterio di riunione globale per l'organizzazione:</span><span class="sxs-lookup"><span data-stu-id="a6225-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="a6225-105">Questo cmdlet richiede attualmente l'utilizzo del modulo di Windows PowerShell per Skype for business.</span><span class="sxs-lookup"><span data-stu-id="a6225-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="a6225-106">Per ottenere il programma di installazione per l'utilizzo di questo cmdlet, vedere Managing policys tramite PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a6225-106">To get setup to use this cmdlet, check out Managing policies via PowerShell.</span></span>

<span data-ttu-id="a6225-107">È possibile configurare un nuovo criterio, che sarà necessario applicare agli utenti.</span><span class="sxs-lookup"><span data-stu-id="a6225-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="a6225-108">Se si modifica il criterio globale, verrà applicato automaticamente agli utenti.</span><span class="sxs-lookup"><span data-stu-id="a6225-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="a6225-109">Per eventuali modifiche ai criteri, è necessario attendere almeno 4 ore e fino a 24 ore per rendere effettive le condizioni.</span><span class="sxs-lookup"><span data-stu-id="a6225-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="a6225-110">Assicurarsi di esaminare la documentazione seguente prima di apportare queste modifiche per comprendere esattamente cosa può essere consentito.</span><span class="sxs-lookup"><span data-stu-id="a6225-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="a6225-111">Informazioni sui controlli dei criteri di lobby riunione dei team</span><span class="sxs-lookup"><span data-stu-id="a6225-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="a6225-112">[Ammetti automaticamente](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) che la gente è un criterio per organizzatore che controlla se gli utenti partecipano a una riunione direttamente o attendono nella lobby finché non vengono ammessi da un utente autenticato.</span><span class="sxs-lookup"><span data-stu-id="a6225-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="a6225-113">[Consenti agli utenti anonimi di avviare una riunione](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) è un criterio per ogni organizzatore che controlla se la gente anonima, inclusi i clienti B2B e federati, è in grado di partecipare alla riunione dell'utente senza un utente autenticato proveniente dall'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="a6225-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="a6225-114">[Consenti agli utenti con accesso esterno di ignorare la lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**prossimamente**) è un criterio per ogni organizzatore che controlla se le persone che accedono tramite telefono accedono alla riunione direttamente o attendono nella lobby, indipendentemente dall'impostazione di **ammetti persone automaticamente** .</span><span class="sxs-lookup"><span data-stu-id="a6225-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="a6225-115">[Consenti agli organizzatori di ignorare le impostazioni della lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**presto disponibile**) è un criterio per ogni organizzatore che controlla se l'organizzatore della riunione può ignorare le impostazioni della lobby che un amministratore ha impostato in modo automatico per consentire agli **utenti** di accedere **in accesso esterno consente agli utenti di ignorare la lobby** quando pianificano una nuova riunione.</span><span class="sxs-lookup"><span data-stu-id="a6225-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="a6225-116">**Nota:** Leggere [Manage meeting Policy in teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) per una panoramica completa dei criteri di riunione di Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="a6225-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
