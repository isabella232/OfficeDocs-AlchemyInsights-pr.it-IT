---
title: Aggiornare i server dei nomi di dominio a Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510288"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="989fc-102">Aggiornare i server dei nomi di dominio a Microsoft</span><span class="sxs-lookup"><span data-stu-id="989fc-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="989fc-103">Nota: la propagazione delle modifiche del server dei nomi può talvolta richiedere fino a 48 ore.</span><span class="sxs-lookup"><span data-stu-id="989fc-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="989fc-104">Per configurare il dominio con Microsoft, è necessario aggiornare i server dei nomi presso il registrar.</span><span class="sxs-lookup"><span data-stu-id="989fc-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="989fc-105">Creare o modificare i record dei server dei nomi nel registrar.</span><span class="sxs-lookup"><span data-stu-id="989fc-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="989fc-106">Passare al sito Web del registrar e trovare l'area in cui è possibile modificare i server dei nomi.</span><span class="sxs-lookup"><span data-stu-id="989fc-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="989fc-107">Creare o modificare due record dei server dei nomi in modo che corrispondano a questi valori:</span><span class="sxs-lookup"><span data-stu-id="989fc-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="989fc-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="989fc-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="989fc-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="989fc-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="989fc-110">Salvare le modifiche.</span><span class="sxs-lookup"><span data-stu-id="989fc-110">Save changes.</span></span>

<span data-ttu-id="989fc-111">È inoltre possibile trovare istruzioni dettagliate in questo articolo: [modificare i server dei nomi per configurare Microsoft 365 con qualsiasi registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="989fc-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  