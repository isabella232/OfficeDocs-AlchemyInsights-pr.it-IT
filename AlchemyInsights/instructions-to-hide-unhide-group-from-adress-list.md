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
# <a name="hide-office-365-group-from-address-list-gal"></a><span data-ttu-id="1e034-102">Nascondi gruppo di Office 365 dall'elenco indirizzi (GAL)</span><span class="sxs-lookup"><span data-stu-id="1e034-102">Hide Office 365 group from address list (GAL)</span></span>

<span data-ttu-id="1e034-103">Per nascondere un gruppo di Office 365 da elenchi di indirizzi (GAL) di client di Exchange (ad esempio Outlook o OWA), utilizzare il seguente comando in EXO Shell:</span><span class="sxs-lookup"><span data-stu-id="1e034-103">To hide an Office 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="1e034-104">Per nascondere il gruppo di Office 365 dalla visibilità ai client di Exchange, utilizzare il seguente comando in EXO Shell:</span><span class="sxs-lookup"><span data-stu-id="1e034-104">To hide the Office 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

