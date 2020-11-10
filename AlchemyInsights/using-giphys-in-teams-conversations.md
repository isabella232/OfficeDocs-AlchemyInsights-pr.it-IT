---
title: Utilizzo di Giphys nelle conversazioni di Teams
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947515"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="86ee9-102">Utilizzo di Giphys nelle conversazioni di Teams</span><span class="sxs-lookup"><span data-stu-id="86ee9-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="86ee9-103">L'accesso Giphys in teams chat è abilitato per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="86ee9-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="86ee9-104">In qualità di amministratore, è possibile controllare se **Giphys è disponibile** per gli utenti [impostando un criterio di messaggistica](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) e assicurando che l'utilizzo di **Giphys nelle conversazioni** sia attivato.</span><span class="sxs-lookup"><span data-stu-id="86ee9-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="86ee9-105">Se gif non funziona come previsto nelle conversazioni dei team, verificare quanto segue:</span><span class="sxs-lookup"><span data-stu-id="86ee9-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="86ee9-106">Il [criterio di messaggistica](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) deve consentire Giphys.</span><span class="sxs-lookup"><span data-stu-id="86ee9-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="86ee9-107">Per verificare l'utilizzo dei cmdlet di PowerShell:</span><span class="sxs-lookup"><span data-stu-id="86ee9-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="86ee9-108">Verificare che sia possibile [gestire i team con PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="86ee9-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="86ee9-109">Eseguire il comando PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) e verificare che **AllowGiphy** sia impostato su **true**.</span><span class="sxs-lookup"><span data-stu-id="86ee9-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="86ee9-110">Se **AllowGiphy** è impostato su **false** , eseguire il seguente comando di PowerShell [set-CsTeamsMessagingPolicy-Identity global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="86ee9-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="86ee9-111">È necessario abilitare le [esperienze collegate facoltative](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) per consentire l'accesso all'URL di Giphy.</span><span class="sxs-lookup"><span data-stu-id="86ee9-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="86ee9-112">Se si dispone di più criteri di messaggistica di team configurati per il tenant, è possibile determinare l'identità del criterio assegnato all'utente interessato con il comando di PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selezionare TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="86ee9-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
