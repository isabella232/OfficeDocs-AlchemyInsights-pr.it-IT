---
title: Limitare l'accesso in SharePoint o OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720686"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="b9dc0-102">Limitare l'accesso in SharePoint o OneDrive</span><span class="sxs-lookup"><span data-stu-id="b9dc0-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="b9dc0-103">In SharePoint e OneDrive, è possibile limitare l'accesso a elementi quali file, cartelle ed elenchi concedendo l'accesso solo ai gruppi o alle persone a cui si desidera accedere.</span><span class="sxs-lookup"><span data-stu-id="b9dc0-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="b9dc0-104">Per impostazione predefinita, le autorizzazioni in SharePoint vengono ereditate dall'alto nella gerarchia.</span><span class="sxs-lookup"><span data-stu-id="b9dc0-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="b9dc0-105">In questo modo un file eredita le autorizzazioni dalla cartella, che eredita le autorizzazioni dalla raccolta, che eredita le autorizzazioni dal sito.</span><span class="sxs-lookup"><span data-stu-id="b9dc0-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="b9dc0-106">È possibile condividere a un livello superiore, ad esempio la condivisione di un intero sito, e quindi interrompere l'ereditarietà se non si desidera condividere tutti gli elementi del sito.</span><span class="sxs-lookup"><span data-stu-id="b9dc0-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="b9dc0-107">Tuttavia, non è consigliabile perché rende più complesse e confuse le autorizzazioni per il futuro.</span><span class="sxs-lookup"><span data-stu-id="b9dc0-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="b9dc0-108">Ecco cosa si potrebbe fare, invece:</span><span class="sxs-lookup"><span data-stu-id="b9dc0-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="b9dc0-109">Se, ad esempio, si desidera condividere tutto il contenuto di una cartella ad eccezione di un file in esso, spostare il file in una nuova posizione che non è condivisa.</span><span class="sxs-lookup"><span data-stu-id="b9dc0-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="b9dc0-110">Se si dispone di due sottocartelle in una cartella e si desidera condividere una sottocartella con i gruppi A e B e consentire l'accesso solo al gruppo a alla seconda sottocartella, condividere la cartella padre con il gruppo A e aggiungere il gruppo B alla prima sottocartella.</span><span class="sxs-lookup"><span data-stu-id="b9dc0-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="b9dc0-111">Interrompere la condivisione di un file o una cartella </span><span class="sxs-lookup"><span data-stu-id="b9dc0-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

