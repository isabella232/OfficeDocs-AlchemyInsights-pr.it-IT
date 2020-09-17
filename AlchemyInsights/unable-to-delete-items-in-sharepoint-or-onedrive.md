---
title: Impossibile eliminare gli elementi in SharePoint o OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806115"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="f14c8-102">Impossibile eliminare gli elementi</span><span class="sxs-lookup"><span data-stu-id="f14c8-102">Unable to delete items</span></span>

<span data-ttu-id="f14c8-103">I criteri di conservazione possono causare questa operazione, è necessario disabilitare o escludere il blocco corrispondente che causa questo problema.</span><span class="sxs-lookup"><span data-stu-id="f14c8-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="f14c8-104">Dopo la rimozione di un criterio di conservazione o di un blocco, potrebbero essere necessarie fino a 24 ore per rendere effettive le modifiche.</span><span class="sxs-lookup"><span data-stu-id="f14c8-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="f14c8-105">Verificare che non vi sia una configurazione dei [criteri di conservazione](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) per l'elemento.</span><span class="sxs-lookup"><span data-stu-id="f14c8-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="f14c8-106">Il sito potrebbe avere superato il limite di archiviazione, aumentare la [quota del sito](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ed eliminare l'elemento.</span><span class="sxs-lookup"><span data-stu-id="f14c8-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="f14c8-107">Verificare che l'elemento non venga [Estratto](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) da un altro utente.</span><span class="sxs-lookup"><span data-stu-id="f14c8-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="f14c8-108">Infine, gli amministratori possono utilizzare [le procedure e i modelli di SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP) che contengono una raccolta di comandi di PowerShell che consentono di eseguire azioni di gestione complesse, ad esempio forza eliminando gli elementi ostinati.</span><span class="sxs-lookup"><span data-stu-id="f14c8-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="f14c8-109">Rimuovi file PNP</span><span class="sxs-lookup"><span data-stu-id="f14c8-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="f14c8-110">Rimuovi cartella PNP</span><span class="sxs-lookup"><span data-stu-id="f14c8-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="f14c8-111">Rimuovi elemento dell'elenco PNP</span><span class="sxs-lookup"><span data-stu-id="f14c8-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="f14c8-112">Rimuovi elenco PNP</span><span class="sxs-lookup"><span data-stu-id="f14c8-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="f14c8-113">Rimuovi campo PNP (colonna)</span><span class="sxs-lookup"><span data-stu-id="f14c8-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)