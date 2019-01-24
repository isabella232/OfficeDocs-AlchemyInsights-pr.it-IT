---
title: Aggiornare i server dei nomi di dominio a Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.openlocfilehash: 81479c4438ce7d981af1312fd4eb7b6ae51ffd42
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475634"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="1290b-102">Aggiornare i server dei nomi di dominio a Office 365</span><span class="sxs-lookup"><span data-stu-id="1290b-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="1290b-103">Nota: Modifiche di nomi talvolta possono richiedere fino a 48 ore per propagare.</span><span class="sxs-lookup"><span data-stu-id="1290b-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="1290b-p101">Per configurare il dominio in Office 365, è necessario aggiornare i server dei nomi nel registrar. Creare o modificare i record dei server dei nomi nel registrar.</span><span class="sxs-lookup"><span data-stu-id="1290b-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="1290b-106">Passare al sito Web del registrar e trovare l'area in cui è possibile modificare i server dei nomi.</span><span class="sxs-lookup"><span data-stu-id="1290b-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="1290b-107">Creare o modificare due record dei server dei nomi in modo che corrispondano a questi valori:</span><span class="sxs-lookup"><span data-stu-id="1290b-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="1290b-108">ns1.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1290b-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="1290b-109">NS2.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1290b-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="1290b-110">Salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="1290b-110">Save changes.</span></span>
    
<span data-ttu-id="1290b-111">Per istruzioni dettagliate, vedere anche questo articolo: [Modificare i server dei nomi per configurare Office 365 con un registrar](https://support.office.com/article/https://support.office.com/en-us/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="1290b-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/https://support.office.com/en-us/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

