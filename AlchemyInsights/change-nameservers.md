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
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736653"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="454d8-102">Aggiornare i server dei nomi di dominio a Office 365</span><span class="sxs-lookup"><span data-stu-id="454d8-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="454d8-103">Nota: la propagazione delle modifiche del server dei nomi può talvolta richiedere fino a 48 ore.</span><span class="sxs-lookup"><span data-stu-id="454d8-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="454d8-p101">Per configurare il dominio in Office 365, è necessario aggiornare i server dei nomi nel registrar. Creare o modificare i record dei server dei nomi nel registrar.</span><span class="sxs-lookup"><span data-stu-id="454d8-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="454d8-106">Passare al sito Web del registrar e trovare l'area in cui è possibile modificare i server dei nomi.</span><span class="sxs-lookup"><span data-stu-id="454d8-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="454d8-107">Creare o modificare due record dei server dei nomi in modo che corrispondano a questi valori:</span><span class="sxs-lookup"><span data-stu-id="454d8-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="454d8-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="454d8-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="454d8-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="454d8-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="454d8-110">Salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="454d8-110">Save changes.</span></span>

<span data-ttu-id="454d8-111">Per istruzioni dettagliate, vedere anche questo articolo: [Modificare i server dei nomi per configurare Office 365 con un registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="454d8-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  