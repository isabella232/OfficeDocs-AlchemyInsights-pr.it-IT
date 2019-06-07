---
title: Impossibile eliminare gli elementi in SharePoint o OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757929"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="9246d-102">Impossibile eliminare gli elementi</span><span class="sxs-lookup"><span data-stu-id="9246d-102">Unable to delete items</span></span>

<span data-ttu-id="9246d-103">Problemi relativi all'eliminazione di elementi?</span><span class="sxs-lookup"><span data-stu-id="9246d-103">Having issues deleting items?</span></span>

- <span data-ttu-id="9246d-104">Assicurarsi sempre di disporre delle [autorizzazioni appropriate](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) per eliminare l'elemento oppure che il tentativo di amministratore di una [raccolta siti](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) sia stato rimosso.</span><span class="sxs-lookup"><span data-stu-id="9246d-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="9246d-105">Verificare che non vi sia una configurazione dei [criteri di conservazione](https://docs.microsoft.com/office365/securitycompliance/retention-policies) per l'elemento.</span><span class="sxs-lookup"><span data-stu-id="9246d-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="9246d-106">Verificare che l'elemento non venga [Estratto](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) da un altro utente.</span><span class="sxs-lookup"><span data-stu-id="9246d-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="9246d-107">Infine, gli amministratori possono utilizzare [le procedure e i modelli di SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) che contengono una raccolta di comandi di PowerShell che consentono di eseguire azioni di gestione complesse, ad esempio forza eliminando gli elementi ostinati.</span><span class="sxs-lookup"><span data-stu-id="9246d-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="9246d-108">Rimuovi file PNP</span><span class="sxs-lookup"><span data-stu-id="9246d-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="9246d-109">Rimuovi cartella PNP</span><span class="sxs-lookup"><span data-stu-id="9246d-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="9246d-110">Rimuovi elemento dell'elenco PNP</span><span class="sxs-lookup"><span data-stu-id="9246d-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="9246d-111">Rimuovi elenco PNP</span><span class="sxs-lookup"><span data-stu-id="9246d-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="9246d-112">Rimuovi campo PNP (colonna)</span><span class="sxs-lookup"><span data-stu-id="9246d-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)