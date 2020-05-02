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
# <a name="private-channels-in-microsoft-teams"></a>Canali privati in Microsoft Teams

Canali privati è una nuova funzionalità di Microsoft teams. Si noti che i canali privati non possono essere convertiti da canali standard o viceversa.

Per informazioni dettagliate sui canali privati, ad esempio le informazioni sulla [creazione di canale privato e l'appartenenza](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) e i [siti di SharePoint di canale privato](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), vedere [private channels in Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Nota:** Poiché la configurazione per la conservazione dei messaggi di canale privato non è ancora supportata, i tenant con i criteri di conservazione abilitati non disporranno di canali privati abilitati per impostazione predefinita. I canali privati possono essere abilitati nell'interfaccia di amministrazione dei team. Si noti inoltre che, sebbene la conservazione dei messaggi di canale privato non sia supportata, è supportata la conservazione dei file condivisi nei canali privati.

**Serve un nuovo proprietario del team?**

Se il proprietario del canale privato lascia, è possibile aggiungere un nuovo proprietario del team tramite teams PowerShell.


- Andare [qui](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) per installare teams PowerShell.

Di seguito è indicato il cmdlet necessario:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Per ulteriori informazioni sui team di PowerShell, vedere [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
