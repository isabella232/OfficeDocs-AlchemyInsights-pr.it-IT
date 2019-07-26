---
title: Cambiare i server dei nomi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902933"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="c0283-102">Aggiornare i server dei nomi di dominio a Office 365</span><span class="sxs-lookup"><span data-stu-id="c0283-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="c0283-103">Nota: la propagazione delle modifiche del server dei nomi può talvolta richiedere fino a 48 ore.</span><span class="sxs-lookup"><span data-stu-id="c0283-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="c0283-p101">Per configurare il dominio in Office 365, è necessario aggiornare i server dei nomi nel registrar. Creare o modificare i record dei server dei nomi nel registrar.</span><span class="sxs-lookup"><span data-stu-id="c0283-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="c0283-106">Passare al sito Web del registrar e trovare l'area in cui è possibile modificare i server dei nomi.</span><span class="sxs-lookup"><span data-stu-id="c0283-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="c0283-107">Creare o modificare due record dei server dei nomi in modo che corrispondano a questi valori:</span><span class="sxs-lookup"><span data-stu-id="c0283-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="c0283-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="c0283-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="c0283-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="c0283-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="c0283-110">Salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="c0283-110">Save changes.</span></span>

<span data-ttu-id="c0283-111">Per istruzioni dettagliate, vedere anche questo articolo: [Modificare i server dei nomi per configurare Office 365 con un registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="c0283-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  