---
title: Creare un messaggio di posta elettronica catch all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712990"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="bdd16-102">Creare un messaggio di posta elettronica catch all</span><span class="sxs-lookup"><span data-stu-id="bdd16-102">Create an email catch all</span></span>

<span data-ttu-id="bdd16-103">L'utilizzo di un catch all è fortemente scoraggiato.</span><span class="sxs-lookup"><span data-stu-id="bdd16-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="bdd16-104">È preferibile fornire un rimbalzo al mittente affinché i mittenti siano a conoscenza del messaggio che non è stato possibile recapitare come indirizzato in modo che possano intervenire.</span><span class="sxs-lookup"><span data-stu-id="bdd16-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="bdd16-105">È inoltre possibile limitare la cassetta postale monitorata solo per rilevare gli indirizzi di posta elettronica precedentemente validi.</span><span class="sxs-lookup"><span data-stu-id="bdd16-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="bdd16-106">Qualsiasi catch tutte le cassette postali riceverà una buona dose di posta indesiderata e potrebbe eventualmente essere compilato se non monitorato.</span><span class="sxs-lookup"><span data-stu-id="bdd16-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="bdd16-107">(Ci sono limiti di ricezione).</span><span class="sxs-lookup"><span data-stu-id="bdd16-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="bdd16-108">Se si decide di procedere, attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="bdd16-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="bdd16-109">Creare un gruppo di distribuzione dinamico & includere "tutti i tipi di destinatari".</span><span class="sxs-lookup"><span data-stu-id="bdd16-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="bdd16-110">Creare una cassetta postale dedicata per la cattura di messaggi di posta elettronica, ad esempio, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="bdd16-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="bdd16-111">Per il dominio specifico, impostare DomainType su "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="bdd16-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="bdd16-112">Se in seguito si rimuove il blocco tutto, assicurarsi di impostare di nuovo il dominio su autorevole.</span><span class="sxs-lookup"><span data-stu-id="bdd16-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="bdd16-113">Creare una regola di trasporto del flusso di posta come indicato di seguito:</span><span class="sxs-lookup"><span data-stu-id="bdd16-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="bdd16-114">Se il mittente è "all'esterno dell'organizzazione"</span><span class="sxs-lookup"><span data-stu-id="bdd16-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="bdd16-115">Reindirizzare il messaggio a Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="bdd16-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="bdd16-116">Eccetto se il destinatario è un membro di allusers@domain.com (il gruppo di distribuzione contiene tutti i membri)</span><span class="sxs-lookup"><span data-stu-id="bdd16-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="bdd16-117">Assicurarsi di verificare che nuove cassette postali vengano aggiunte al gruppo di distribuzione dinamico</span><span class="sxs-lookup"><span data-stu-id="bdd16-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
