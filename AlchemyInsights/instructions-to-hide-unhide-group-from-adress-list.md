---
title: Istruzioni per nascondere/visualizzare un gruppo dall'elenco di indirizzi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580013"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Nascondi gruppo di Microsoft 365 dall'elenco indirizzi (GAL)

Per nascondere un gruppo di Microsoft 365 dall'elenco indirizzi (GAL) dei client di Exchange (ad esempio Outlook o OWA), utilizzare il seguente comando in EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Per nascondere il gruppo di Microsoft 365 da essere visibile ai client di Exchange, utilizzare il seguente comando in EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

