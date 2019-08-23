---
title: Impossibile eliminare gli elementi in SharePoint o OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558657"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="71a01-102">Impossibile eliminare gli elementi</span><span class="sxs-lookup"><span data-stu-id="71a01-102">Unable to delete items</span></span>

<span data-ttu-id="71a01-103">Problemi relativi all'eliminazione di elementi di SharePoint</span><span class="sxs-lookup"><span data-stu-id="71a01-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="71a01-104">Assicurarsi sempre di disporre delle [autorizzazioni appropriate](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) per eliminare l'elemento oppure che il tentativo di amministratore di una [raccolta siti](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) sia stato rimosso.</span><span class="sxs-lookup"><span data-stu-id="71a01-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="71a01-105">Verificare che non vi sia una configurazione dei [criteri di conservazione](https://docs.microsoft.com/office365/securitycompliance/retention-policies) per l'elemento.</span><span class="sxs-lookup"><span data-stu-id="71a01-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="71a01-106">Verificare che l'elemento non venga [Estratto](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) da un altro utente.</span><span class="sxs-lookup"><span data-stu-id="71a01-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="71a01-107">Infine, gli amministratori possono utilizzare [le procedure e i modelli di SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) che contengono una raccolta di comandi di PowerShell che consentono di eseguire azioni di gestione complesse, ad esempio forza eliminando gli elementi ostinati.</span><span class="sxs-lookup"><span data-stu-id="71a01-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="71a01-108">Rimuovi file PNP</span><span class="sxs-lookup"><span data-stu-id="71a01-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="71a01-109">Rimuovi cartella PNP</span><span class="sxs-lookup"><span data-stu-id="71a01-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="71a01-110">Rimuovi elemento dell'elenco PNP</span><span class="sxs-lookup"><span data-stu-id="71a01-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="71a01-111">Rimuovi elenco PNP</span><span class="sxs-lookup"><span data-stu-id="71a01-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="71a01-112">Rimuovi campo PNP (colonna)</span><span class="sxs-lookup"><span data-stu-id="71a01-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)