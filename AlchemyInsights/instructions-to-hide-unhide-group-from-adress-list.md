---
title: Istruzioni per nascondere/mostrare il gruppo dall'elenco indirizzi
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
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926249"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Nascondere Microsoft 365 gruppo dall'elenco indirizzi globale

Per nascondere un Microsoft 365 di indirizzi globale (GAL) di client Exchange (ad esempio Outlook o OWA), utilizzare il comando seguente nella shell exO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Per nascondere il gruppo Microsoft 365 visibile ai client Exchange, utilizzare il comando seguente nella shell EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

