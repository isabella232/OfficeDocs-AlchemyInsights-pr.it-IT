---
title: Aggiornare i server dei nomi di dominio a Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742184"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="8f089-102">Aggiornare i server dei nomi di dominio a Office 365</span><span class="sxs-lookup"><span data-stu-id="8f089-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="8f089-103">Nota: la propagazione delle modifiche del server dei nomi può talvolta richiedere fino a 48 ore.</span><span class="sxs-lookup"><span data-stu-id="8f089-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="8f089-p101">Per configurare il dominio in Office 365, è necessario aggiornare i server dei nomi nel registrar. Creare o modificare i record dei server dei nomi nel registrar.</span><span class="sxs-lookup"><span data-stu-id="8f089-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="8f089-106">Passare al sito Web del registrar e trovare l'area in cui è possibile modificare i server dei nomi.</span><span class="sxs-lookup"><span data-stu-id="8f089-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="8f089-107">Creare o modificare due record dei server dei nomi in modo che corrispondano a questi valori:</span><span class="sxs-lookup"><span data-stu-id="8f089-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="8f089-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="8f089-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="8f089-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="8f089-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="8f089-110">Salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="8f089-110">Save changes.</span></span>

<span data-ttu-id="8f089-111">Per istruzioni dettagliate, vedere anche questo articolo: [Modificare i server dei nomi per configurare Office 365 con un registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="8f089-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  