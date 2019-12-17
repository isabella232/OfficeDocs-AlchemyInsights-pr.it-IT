---
title: Risoluzione dei problemi relativi ai messaggi di accesso negato
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050709"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="510da-102">Risoluzione dei problemi relativi ai messaggi di accesso negato</span><span class="sxs-lookup"><span data-stu-id="510da-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="510da-103">Se qualcuno ha ricevuto un messaggio di accesso negato a una cartella condivisa in SharePoint, l'amministratore della raccolta siti potrebbe aver abilitato la modalità di blocco delle autorizzazioni utente con accesso limitato.</span><span class="sxs-lookup"><span data-stu-id="510da-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="510da-104">Per disattivare questa opzione:</span><span class="sxs-lookup"><span data-stu-id="510da-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="510da-105">Passare al sito, fare clic sull'icona impostazioni e quindi su **Impostazioni sito**.</span><span class="sxs-lookup"><span data-stu-id="510da-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="510da-106">In **Amministrazione raccolta siti** fare clic su **Caratteristiche raccolta siti**.</span><span class="sxs-lookup"><span data-stu-id="510da-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="510da-107">Accanto alla **modalità di blocco delle autorizzazioni utente con accesso limitato**, fare clic su **Disattiva**.</span><span class="sxs-lookup"><span data-stu-id="510da-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="510da-108">Se il sito è un sito di pubblicazione, è possibile che si verifichi un messaggio di accesso negato anche per le cartelle condivise.</span><span class="sxs-lookup"><span data-stu-id="510da-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="510da-109">Per informazioni, vedere [accesso negato quando si accede a una cartella condivisa](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="510da-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="510da-110">Se un utente ha ricevuto un messaggio di accesso negato quando si tenta di visualizzare le richieste di accesso, è necessario aggiungerlo come amministratore della raccolta siti o come membro del gruppo proprietari per il sito.</span><span class="sxs-lookup"><span data-stu-id="510da-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="510da-111">Per altre informazioni, vedere [Access denied to Access requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="510da-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="510da-112">Se un utente ha ricevuto un messaggio di accesso negato dopo che è stato rimosso da Active Directory locale e quindi è stato aggiunto indietro, vedere [accesso negato quando un account utente viene sincronizzato con Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="510da-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

