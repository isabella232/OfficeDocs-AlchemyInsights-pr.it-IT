---
title: Creare un messaggio di posta elettronica catch all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816204"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="c64ad-102">Creare un messaggio di posta elettronica catch all</span><span class="sxs-lookup"><span data-stu-id="c64ad-102">Create an email catch all</span></span>

<span data-ttu-id="c64ad-103">L'uso di un catch all è fortemente sconsigliato.</span><span class="sxs-lookup"><span data-stu-id="c64ad-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="c64ad-104">È meglio fornire un rimbalzo al mittente, in modo che i mittenti sappiano che il messaggio non può essere recapitato come indirizzato in modo che possano agire.</span><span class="sxs-lookup"><span data-stu-id="c64ad-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="c64ad-105">È inoltre possibile limitare la cassetta postale monitorata solo agli indirizzi di posta elettronica validi in precedenza.</span><span class="sxs-lookup"><span data-stu-id="c64ad-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="c64ad-106">Qualsiasi blocco di tutte le cassette postali riceverà una buona quantità di posta indesiderata e potrebbe eventualmente riempirsi se non strettamente monitorato.</span><span class="sxs-lookup"><span data-stu-id="c64ad-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="c64ad-107">Sono previsti limiti di ricezione.</span><span class="sxs-lookup"><span data-stu-id="c64ad-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="c64ad-108">Se si decide di procedere, attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="c64ad-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="c64ad-109">Creare un gruppo di distribuzione dinamico & "Tutti i tipi di destinatari".</span><span class="sxs-lookup"><span data-stu-id="c64ad-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="c64ad-110">Creare una cassetta postale dedicata per intercettare i messaggi di posta elettronica, ad esempio, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="c64ad-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="c64ad-111">Per il dominio specifico, imposta DomainType su "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="c64ad-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="c64ad-112">Se in seguito si rimuovono tutti i blocchi, assicurarsi di impostare nuovamente il dominio su Autorevole.</span><span class="sxs-lookup"><span data-stu-id="c64ad-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="c64ad-113">Creare una regola di trasporto Del flusso di posta come segue:</span><span class="sxs-lookup"><span data-stu-id="c64ad-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="c64ad-114">Se il mittente è "Esterno all'organizzazione"</span><span class="sxs-lookup"><span data-stu-id="c64ad-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="c64ad-115">Reindirizzare il messaggio a Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="c64ad-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="c64ad-116">Tranne se il destinatario è un membro di allusers@domain.com (il gruppo di distribuzione contiene tutti i membri)</span><span class="sxs-lookup"><span data-stu-id="c64ad-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="c64ad-117">Verificare che le nuove cassette postali siano aggiunte al gruppo di distribuzione dinamico</span><span class="sxs-lookup"><span data-stu-id="c64ad-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
