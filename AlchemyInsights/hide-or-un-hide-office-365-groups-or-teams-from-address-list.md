---
title: Nascondere o rendere visibili gruppi/team di Office 365 dall'elenco di indirizzi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225441"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Nascondere o rendere visibili gruppi/team di Office 365 dall'elenco di indirizzi

Usare il comando EXO PowerShell seguente per nascondere o rendere visibile gruppi/team di Office 365 da elenchi di indirizzi (GAL) di client Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Usare il comando EXO PowerShell seguente per nascondere o rendere visibile gruppi/team di Office365 da client Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Per istruzioni dettagliate, vedere [Nascondere i gruppi di Office 365 dai client GAL e Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
