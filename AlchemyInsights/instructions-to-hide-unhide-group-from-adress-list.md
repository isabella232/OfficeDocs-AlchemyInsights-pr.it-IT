---
title: Istruzioni per nascondere/visualizzare un gruppo dall'elenco di indirizzi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663013"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Nascondi gruppo di Microsoft 365 dall'elenco indirizzi (GAL)

Per nascondere un gruppo di Microsoft 365 dall'elenco indirizzi (GAL) dei client di Exchange (ad esempio Outlook o OWA), utilizzare il seguente comando in EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Per nascondere il gruppo di Microsoft 365 da essere visibile ai client di Exchange, utilizzare il seguente comando in EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

