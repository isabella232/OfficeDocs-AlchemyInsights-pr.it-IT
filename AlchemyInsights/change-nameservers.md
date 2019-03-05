---
title: Modificare i server dei nomi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 61c4c5e43a247679bf18fd3861dd98fbe9a7b3eb
ms.sourcegitcommit: f1c96fd3890d4e211f7d6bf73b9105fdaab2e11c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2019
ms.locfileid: "30405327"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="1d7f6-102">Aggiornare i server dei nomi di dominio a Office 365</span><span class="sxs-lookup"><span data-stu-id="1d7f6-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="1d7f6-103">Note: le modifiche dei server dei nomi possono talvolta richiedere fino a 48 ore per propagarsi.</span><span class="sxs-lookup"><span data-stu-id="1d7f6-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="1d7f6-p101">Per configurare il dominio in Office 365, è necessario aggiornare i server dei nomi nel registrar. Creare o modificare i record dei server dei nomi nel registrar.</span><span class="sxs-lookup"><span data-stu-id="1d7f6-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="1d7f6-106">Passare al sito Web del registrar e trovare l'area in cui è possibile modificare i server dei nomi.</span><span class="sxs-lookup"><span data-stu-id="1d7f6-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="1d7f6-107">Creare o modificare due record dei server dei nomi in modo che corrispondano a questi valori:</span><span class="sxs-lookup"><span data-stu-id="1d7f6-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="1d7f6-108">ns1.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1d7f6-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="1d7f6-109">NS2.BDM.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="1d7f6-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="1d7f6-110">Salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="1d7f6-110">Save changes.</span></span>
    
<span data-ttu-id="1d7f6-111">Per istruzioni dettagliate, vedere anche questo articolo: [Modificare i server dei nomi per configurare Office 365 con un registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="1d7f6-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

