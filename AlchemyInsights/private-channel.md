---
title: Canale privato
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005442"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="8fe5a-102">Canali privati in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="8fe5a-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="8fe5a-103">Canali privati è una nuova funzionalità di Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="8fe5a-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="8fe5a-104">Si noti che i canali privati non possono essere convertiti da canali standard o viceversa.</span><span class="sxs-lookup"><span data-stu-id="8fe5a-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="8fe5a-105">Per informazioni dettagliate sui canali privati, ad esempio le informazioni sulla [creazione di canale privato e l'appartenenza](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) e i [siti di SharePoint di canale privato](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), vedere [private channels in Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="8fe5a-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="8fe5a-106">**Nota:** Poiché la configurazione per la conservazione dei messaggi di canale privato non è ancora supportata, i tenant con i criteri di conservazione abilitati non disporranno di canali privati abilitati per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="8fe5a-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="8fe5a-107">I canali privati possono essere abilitati nell'interfaccia di amministrazione dei team.</span><span class="sxs-lookup"><span data-stu-id="8fe5a-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="8fe5a-108">Si noti inoltre che, sebbene la conservazione dei messaggi di canale privato non sia supportata, è supportata la conservazione dei file condivisi nei canali privati.</span><span class="sxs-lookup"><span data-stu-id="8fe5a-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="8fe5a-109">**Serve un nuovo proprietario del team?**</span><span class="sxs-lookup"><span data-stu-id="8fe5a-109">**Need a new team owner?**</span></span>

<span data-ttu-id="8fe5a-110">Se il proprietario del canale privato lascia, è possibile aggiungere un nuovo proprietario del team tramite teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8fe5a-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="8fe5a-111">Andare [qui](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) per installare teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8fe5a-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="8fe5a-112">Di seguito è indicato il cmdlet necessario:</span><span class="sxs-lookup"><span data-stu-id="8fe5a-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="8fe5a-113">Per ulteriori informazioni sui team di PowerShell, vedere [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="8fe5a-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
