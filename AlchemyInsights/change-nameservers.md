---
title: Cambiare i server dei nomi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508092"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="b9e96-102">Aggiornare i server dei nomi di dominio a Microsoft</span><span class="sxs-lookup"><span data-stu-id="b9e96-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="b9e96-103">Nota: la propagazione delle modifiche del server dei nomi può talvolta richiedere fino a 48 ore.</span><span class="sxs-lookup"><span data-stu-id="b9e96-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="b9e96-p101">Per configurare il dominio in Microsoft 365, è necessario aggiornare i server dei nomi nel registrar. Creare o modificare i record dei server dei nomi nel registrar.</span><span class="sxs-lookup"><span data-stu-id="b9e96-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="b9e96-106">Passare al sito Web del registrar e trovare l'area in cui è possibile modificare i server dei nomi.</span><span class="sxs-lookup"><span data-stu-id="b9e96-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="b9e96-107">Creare o modificare due record dei server dei nomi in modo che corrispondano a questi valori:</span><span class="sxs-lookup"><span data-stu-id="b9e96-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="b9e96-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="b9e96-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="b9e96-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="b9e96-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="b9e96-110">Salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="b9e96-110">Save changes.</span></span>

<span data-ttu-id="b9e96-111">Per istruzioni dettagliate, vedere anche questo articolo: [Modificare i server dei nomi con un registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="b9e96-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  