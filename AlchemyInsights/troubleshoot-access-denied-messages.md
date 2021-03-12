---
title: Risoluzione dei problemi relativi ai messaggi di accesso negato
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704898"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="59b71-102">Risoluzione dei problemi relativi ai messaggi di accesso negato</span><span class="sxs-lookup"><span data-stu-id="59b71-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="59b71-103">Se un utente ha ricevuto un messaggio "Accesso negato" a una cartella condivisa in SharePoint, l'amministratore della raccolta siti potrebbe aver abilitato la "modalità di blocco delle autorizzazioni utente con accesso limitato".</span><span class="sxs-lookup"><span data-stu-id="59b71-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="59b71-104">Per disattivare questa opzione:</span><span class="sxs-lookup"><span data-stu-id="59b71-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="59b71-105">Passare al sito, fare clic sull'icona Impostazioni e quindi su **Impostazioni sito.**</span><span class="sxs-lookup"><span data-stu-id="59b71-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="59b71-106">In **Amministrazione raccolta siti** fare clic su **Caratteristiche raccolta siti**.</span><span class="sxs-lookup"><span data-stu-id="59b71-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="59b71-107">Accanto a **Modalità di blocco delle autorizzazioni utente** con accesso limitato fare clic su **Disattiva.**</span><span class="sxs-lookup"><span data-stu-id="59b71-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="59b71-108">È inoltre possibile che per le cartelle condivise si verifichi un messaggio di accesso negato se il sito è un sito di pubblicazione.</span><span class="sxs-lookup"><span data-stu-id="59b71-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="59b71-109">Per informazioni, vedere [Accesso negato quando si accede a una cartella condivisa.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)</span><span class="sxs-lookup"><span data-stu-id="59b71-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="59b71-110">Se un utente ha ricevuto un messaggio "Accesso negato" quando tenta di visualizzare le richieste di accesso, l'utente deve essere aggiunto come amministratore della raccolta siti o come membro del gruppo Proprietari del sito.</span><span class="sxs-lookup"><span data-stu-id="59b71-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="59b71-111">Per altre info, vedi [l'elenco Access Denied to Access Requests.](https://go.microsoft.com/fwlink/?linkid=2004220)</span><span class="sxs-lookup"><span data-stu-id="59b71-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="59b71-112">Se un utente ha ricevuto un messaggio "Accesso negato" dopo essere stato rimosso da Active Directory locale e quindi aggiunto nuovamente, vedere Accesso negato quando un account utente viene sincronizzato con [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)</span><span class="sxs-lookup"><span data-stu-id="59b71-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

