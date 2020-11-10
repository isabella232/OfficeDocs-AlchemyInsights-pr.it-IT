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
# <a name="using-giphys-in-teams-conversations"></a>Utilizzo di Giphys nelle conversazioni di Teams

L'accesso Giphys in teams chat è abilitato per impostazione predefinita. In qualità di amministratore, è possibile controllare se **Giphys è disponibile** per gli utenti [impostando un criterio di messaggistica](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) e assicurando che l'utilizzo di **Giphys nelle conversazioni** sia attivato.

Se gif non funziona come previsto nelle conversazioni dei team, verificare quanto segue:

Il [criterio di messaggistica](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) deve consentire Giphys. Per verificare l'utilizzo dei cmdlet di PowerShell:

- Verificare che sia possibile [gestire i team con PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Eseguire il comando PowerShell [Get-CsTeamsMessagingPolicy-Identity global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) e verificare che **AllowGiphy** sia impostato su **true**.
- Se **AllowGiphy** è impostato su **false** , eseguire il seguente comando di PowerShell [set-CsTeamsMessagingPolicy-Identity global-AllowGiphy $true](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

È necessario abilitare le [esperienze collegate facoltative](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) per consentire l'accesso all'URL di Giphy.

> [!NOTE]
> Se si dispone di più criteri di messaggistica di team configurati per il tenant, è possibile determinare l'identità del criterio assegnato all'utente interessato con il comando di PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selezionare TeamsMessagingPolicy.
