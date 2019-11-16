---
title: Protezione da posta indesiderata 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672437"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="bddfe-102">Risolvere i problemi di recapito per il codice di errore 550 5.4.1 inoltro accesso negato</span><span class="sxs-lookup"><span data-stu-id="bddfe-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="bddfe-103">Questo problema si verifica quando si verifica [se un indirizzo di posta elettronica è valido per impedire effetto palla quando si](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) immette la rete di Office 365.</span><span class="sxs-lookup"><span data-stu-id="bddfe-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="bddfe-104">Provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="bddfe-104">Try the following:</span></span>

1. <span data-ttu-id="bddfe-105">Determinare se il problema è specifico di un intero dominio o di un singolo indirizzo di posta elettronica:</span><span class="sxs-lookup"><span data-stu-id="bddfe-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="bddfe-106">Intero dominio: in alcuni casi il dominio deve essere sincronizzato; provare [a impostare il dominio su Internal e quindi di nuovo su autorevole](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="bddfe-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="bddfe-107">Indirizzo di posta elettronica singolo: a volte l'indirizzo deve essere sincronizzato; la modifica dell'indirizzo proxy SMTP e quindi la modifica di nuovo può essere utile.</span><span class="sxs-lookup"><span data-stu-id="bddfe-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="bddfe-108">Determinare se il problema è specifico di un gruppo o di una cartella pubblica.</span><span class="sxs-lookup"><span data-stu-id="bddfe-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="bddfe-109">Per alcuni tipi di oggetto, è possibile che gli oggetti debbano essere creati manualmente in Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bddfe-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="bddfe-110">Se si ha bisogno di ulteriore assistenza, aprire un ticket di supporto e specificare l'ambito del problema (includidng il tipo di oggetto a cui si sta inviando), in modo da potervi aiutare meglio.</span><span class="sxs-lookup"><span data-stu-id="bddfe-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>