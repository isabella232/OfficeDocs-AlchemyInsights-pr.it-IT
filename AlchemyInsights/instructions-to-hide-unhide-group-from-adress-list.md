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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768930"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Nascondi gruppo di Office 365 dall'elenco indirizzi (GAL)

Per nascondere un gruppo di Office 365 da elenchi di indirizzi (GAL) di client di Exchange (ad esempio Outlook o OWA), utilizzare il seguente comando in EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Per nascondere il gruppo di Office 365 dalla visibilità ai client di Exchange, utilizzare il seguente comando in EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

