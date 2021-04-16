---
title: Nascondere o mostrare i gruppi/team di Office 365 nell'elenco di indirizzi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811460"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Nascondere o mostrare i gruppi/team di Office 365 nell'elenco di indirizzi

Usare il comando EXO PowerShell seguente per nascondere o mostrare i gruppi/team di Office 365 negli elenchi di indirizzi globali dei client Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Usare il comando EXO PowerShell seguente per nascondere o mostrare i gruppi/team di Office365 nei client Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Per istruzioni dettagliate, vedere [Nascondere i gruppi di Office 365 negli elenchi di indirizzi globali e nei client Exchange](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
