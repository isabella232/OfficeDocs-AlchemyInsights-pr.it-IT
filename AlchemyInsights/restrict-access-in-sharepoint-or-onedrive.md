---
title: Limitare l'accesso in SharePoint o OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475779"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="8b279-102">Limitare l'accesso in SharePoint o OneDrive</span><span class="sxs-lookup"><span data-stu-id="8b279-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="8b279-p101">In SharePoint e OneDrive, limitare l'accesso a elementi quali elenchi, cartelle e i file per concedere l'accesso solo ai gruppi o più persone che si desidera possano accedervi. Per impostazione predefinita, le autorizzazioni di SharePoint ereditate da up superiore della gerarchia. Un file in modo eredita le autorizzazioni dalla cartella che eredita le autorizzazioni dalla raccolta, che eredita le autorizzazioni dal sito.</span><span class="sxs-lookup"><span data-stu-id="8b279-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="8b279-p102">È possibile condividere un livello superiore (ad esempio condivisione di un intero sito) e quindi interrompere l'ereditarietà se non si desidera condividere tutti gli elementi nel sito. Tuttavia, non raccomandiamo questa, semplifica la gestione autorizzazioni più complessa e confusione in futuro. Ecco cosa si può fare invece:</span><span class="sxs-lookup"><span data-stu-id="8b279-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="8b279-109">Se, ad esempio, si desidera condividere tutto il contenuto di una cartella ad eccezione di un file, spostare il file in una nuova posizione che non è condiviso.</span><span class="sxs-lookup"><span data-stu-id="8b279-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="8b279-110">Se si dispone di due sottocartelle in una cartella e si desidera condividere una sottocartella con i gruppi A e B e consentire l'accesso del gruppo in alla seconda sottocartella, condividere la cartella padre del gruppo e aggiungere il gruppo B per la prima sottocartella.</span><span class="sxs-lookup"><span data-stu-id="8b279-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="8b279-111">Interrompere la condivisione file o cartelle</span><span class="sxs-lookup"><span data-stu-id="8b279-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

