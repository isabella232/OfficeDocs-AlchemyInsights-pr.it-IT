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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104312"
---
# <a name="using-giphys-in-teams-conversations"></a>Uso di Giphys nelle Teams conversazioni

Giphys access in Teams chat è abilitato per impostazione predefinita. In qualità di amministratore, puoi controllare se Giphys è disponibile per gli utenti impostando un criterio di messaggistica e verificando che **l'opzione Usa Giphys nelle** conversazioni sia [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) **attivata.**

Se le GIF non funzionano come previsto nelle Teams, verificare:

Il [criterio di messaggistica](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) deve consentire Giphys. Per verificare tramite i cmdlet di PowerShell:

- Verificare che sia possibile [gestire Teams con PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Eseguire il comando PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) e verificare che **AllowGiphy** sia impostato su **TRUE.**
- Se **AllowGiphy è** impostato su **FALSE,** eseguire il seguente comando di PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Le esperienze connesse](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) facoltative devono essere abilitate per consentire l'accesso all'URL Giphy.

> [!NOTE]
> Se per il tenant sono configurati più criteri di messaggistica Teams, è possibile determinare l'identità del criterio assegnato all'utente in impatto con il comando PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Selezionare TeamsMessagingPolicy.
