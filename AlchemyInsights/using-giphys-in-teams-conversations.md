---
title: Uso di Giphys nelle Teams conversazioni
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323524"
---
# <a name="using-giphys-in-teams-conversations"></a>Uso di Giphys nelle Teams conversazioni

Giphys access in Teams chat è abilitato per impostazione predefinita. L'amministratore può controllare se Giphys è [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) disponibile per gli utenti impostando un criterio di messaggistica e verificando che **l'opzione Usa Giphys nelle** conversazioni sia **attivata.**

Se le GIF non funzionano come previsto nelle Teams conversazioni, verificare:

Il [criterio di messaggistica](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) deve consentire Giphys. Per verificare tramite i cmdlet di PowerShell:

- Verificare che sia possibile [gestire Teams con PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Eseguire il comando PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) e verificare che **AllowGiphy** sia impostato su **TRUE.**
- Se **AllowGiphy è** impostato su **FALSE,** eseguire il seguente comando di PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Le esperienze connesse](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) facoltative devono essere abilitate per consentire l'accesso all'URL Giphy.

**Nota:** se sono configurati più criteri di messaggistica Teams per il tenant, è possibile determinare l'identità del criterio assegnato all'utente in impatto con il comando PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selezionare TeamsMessagingPolicy.
