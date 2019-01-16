---
title: Risolvere i messaggi di accesso negato
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/15/2019
ms.locfileid: "28296492"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="ed397-102">Risolvere i messaggi di accesso negato</span><span class="sxs-lookup"><span data-stu-id="ed397-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="ed397-p101">Se si dispone di un messaggio "Accesso negato" in una cartella condivisa, l'amministratore della raccolta siti sono abilitati "accesso limitato utente autorizzazione modalità di blocco." Per disattivare questa funzionalità:</span><span class="sxs-lookup"><span data-stu-id="ed397-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="ed397-105">Passare al sito, fare clic sull'icona impostazioni e quindi fare clic su **Impostazioni sito**.</span><span class="sxs-lookup"><span data-stu-id="ed397-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="ed397-106">In **Amministrazione raccolta siti** fare clic su **Caratteristiche raccolta siti**.</span><span class="sxs-lookup"><span data-stu-id="ed397-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="ed397-107">Accanto alla **modalità di blocco dell'autorizzazione utente ad accesso limitato**, fare clic su **Disattiva**.</span><span class="sxs-lookup"><span data-stu-id="ed397-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="ed397-p102">Messaggio accesso negato può inoltre verificarsi per le cartelle condivise se il sito è un sito di pubblicazione. Per informazioni, vedere [Accesso negato quando si accede a una cartella condivisa](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="ed397-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="ed397-p103">Se un utente dispone di un messaggio "Accesso negato" durante il tentativo di visualizzare le richieste di accesso, l'utente deve essere aggiunti come amministratori della raccolta siti o un membro del gruppo proprietari del sito. Per ulteriori informazioni, vedere [Accesso negato a elenco Access Requests](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="ed397-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="ed397-112">Se un utente ha ricevuto un messaggio "Accesso negato" dopo che sono stati rimossi da Active Directory locale e quindi nuovamente aggiunto, vedere [Accesso negato quando un account utente viene sincronizzato con Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="ed397-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

