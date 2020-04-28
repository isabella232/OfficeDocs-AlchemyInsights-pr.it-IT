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
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908348"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Nascondi gruppo di Microsoft 365 dall'elenco indirizzi (GAL)

Per nascondere un gruppo di Microsoft 365 dagli elenchi di indirizzi (GAL) dei client di Exchange (ad esempio Outlook o OWA), utilizzare il seguente comando in EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Per nascondere il gruppo di Microsoft 365 da essere visibile ai client di Exchange, utilizzare il seguente comando in EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

