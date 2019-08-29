---
title: Aggiornare i record DNS per mantenere il proprio sito Web con l'attuale provider di hosting
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665764"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="8c04f-102">Aggiornare i record DNS per mantenere il proprio sito Web con l'attuale provider di hosting</span><span class="sxs-lookup"><span data-stu-id="8c04f-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="8c04f-103">Nell'interfaccia di amministrazione di Microsoft 365 passare alla pagina **installazione** > [domini](https://portal.office.com/adminportal/home#/Domains) e nell'elenco dei domini selezionare il dominio che si sta utilizzando per il sito Web.</span><span class="sxs-lookup"><span data-stu-id="8c04f-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="8c04f-104">Selezionare **+ Nuovo record personalizzato** e immettere quanto segue:</span><span class="sxs-lookup"><span data-stu-id="8c04f-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="8c04f-105">Per **Tipo di DNS** immettere: **A (Indirizzo)**</span><span class="sxs-lookup"><span data-stu-id="8c04f-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="8c04f-106">Per **Nome host o alias** digitare **@**</span><span class="sxs-lookup"><span data-stu-id="8c04f-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="8c04f-107">Per **Indirizzo IP** digitare l'indirizzo IP presso cui il sito Web è attualmente ospitato, ad esempio 172.16.140.1.</span><span class="sxs-lookup"><span data-stu-id="8c04f-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="8c04f-p101">Deve essere un indirizzo IP  *statico*  , non  *dinamico*  , per il sito Web. Contattare il provider in cui è ospitato il sito Web per verificare che sia possibile ottenere un indirizzo IP statico per il sito Web pubblico.</span><span class="sxs-lookup"><span data-stu-id="8c04f-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="8c04f-110">Selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="8c04f-110">Select **Save**.</span></span>

<span data-ttu-id="8c04f-111">È anche possibile creare un record CNAME per aiutare i clienti a trovare il sito Web.</span><span class="sxs-lookup"><span data-stu-id="8c04f-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="8c04f-112">Selezionare **+ Nuovo record personalizzato** e immettere quanto segue:</span><span class="sxs-lookup"><span data-stu-id="8c04f-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="8c04f-113">Per **Tipo di DNS** immettere: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="8c04f-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="8c04f-114">Per **Nome host o alias** digitare **www**</span><span class="sxs-lookup"><span data-stu-id="8c04f-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="8c04f-115">Per **Indirizzo di puntamento** digitare il nome di dominio completo (FQDN) del sito Web, ad esempio contoso.com).</span><span class="sxs-lookup"><span data-stu-id="8c04f-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="8c04f-116">Selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="8c04f-116">Select **Save**.</span></span>
