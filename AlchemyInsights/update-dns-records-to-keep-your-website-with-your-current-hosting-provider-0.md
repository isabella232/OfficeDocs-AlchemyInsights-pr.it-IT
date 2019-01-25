---
title: Aggiornare i record DNS per mantenere il proprio sito Web con l'attuale provider di hosting
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475856"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="f3219-102">Aggiornare i record DNS per mantenere il proprio sito Web con l'attuale provider di hosting</span><span class="sxs-lookup"><span data-stu-id="f3219-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="f3219-103">Nell'elenco dei domini della pagina [Domini](https://portal.office.com/adminportal/home#/Domains) selezionare il dominio usato per il sito Web, quindi selezionare **Impostazioni DNS** nel riquadro di gestione.</span><span class="sxs-lookup"><span data-stu-id="f3219-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="f3219-104">Selezionare **+ Nuovo record personalizzato** e immettere quanto segue:</span><span class="sxs-lookup"><span data-stu-id="f3219-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="f3219-105">Per **Tipo di DNS** immettere: **A (Indirizzo)**</span><span class="sxs-lookup"><span data-stu-id="f3219-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="f3219-106">Per **Nome host o alias** digitare **@**</span><span class="sxs-lookup"><span data-stu-id="f3219-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="f3219-107">Per **Indirizzo IP** digitare l'indirizzo IP presso cui il sito Web è attualmente ospitato, ad esempio 172.16.140.1.</span><span class="sxs-lookup"><span data-stu-id="f3219-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="f3219-p101">Deve essere un indirizzo IP  *statico*  , non  *dinamico*  , per il sito Web. Contattare il provider in cui è ospitato il sito Web per verificare che sia possibile ottenere un indirizzo IP statico per il sito Web pubblico.</span><span class="sxs-lookup"><span data-stu-id="f3219-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="f3219-110">Selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="f3219-110">Select **Save**.</span></span> 
    
<span data-ttu-id="f3219-111">È anche possibile creare un record CNAME per aiutare i clienti a trovare il sito Web.</span><span class="sxs-lookup"><span data-stu-id="f3219-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="f3219-112">Selezionare **+ Nuovo record personalizzato** e immettere quanto segue:</span><span class="sxs-lookup"><span data-stu-id="f3219-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="f3219-113">Per **Tipo di DNS** immettere: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="f3219-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="f3219-114">Per **Nome host o alias** digitare **www**</span><span class="sxs-lookup"><span data-stu-id="f3219-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="f3219-115">Per **Indirizzo di puntamento** digitare il nome di dominio completo (FQDN) del sito Web, ad esempio contoso.com).</span><span class="sxs-lookup"><span data-stu-id="f3219-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="f3219-116">Selezionare **Salva**.</span><span class="sxs-lookup"><span data-stu-id="f3219-116">Select **Save**.</span></span> 
    

