---
title: Criterio di condivisione del calendario 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373003"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="4c781-102">Errore del criterio durante la condivisione di un calendario</span><span class="sxs-lookup"><span data-stu-id="4c781-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="4c781-103">Eseguire una delle operazioni seguenti, a seconda dei casi, per la situazione:</span><span class="sxs-lookup"><span data-stu-id="4c781-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="4c781-104">Connettersi a Exchange Online tramite Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4c781-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="4c781-105">Per ulteriori informazioni, vedere [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4c781-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="4c781-106">Nel server locale, aprire Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="4c781-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="4c781-107">Determinare il criterio di condivisione assegnato all'utente.</span><span class="sxs-lookup"><span data-stu-id="4c781-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="4c781-108">A tale scopo, eseguire il comando riportato di seguito e prendere nota del criterio restituito:</span><span class="sxs-lookup"><span data-stu-id="4c781-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="4c781-109">Aggiornare il criterio di condivisione per l'utente.</span><span class="sxs-lookup"><span data-stu-id="4c781-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="4c781-110">A tale scopo, attieniti alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="4c781-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="4c781-111">Aprire l'interfaccia di amministrazione di Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c781-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="4c781-112">Fare clic su **organizzazione**e quindi fare doppio clic sul criterio assegnato all'utente in **Condivisione singola**.</span><span class="sxs-lookup"><span data-stu-id="4c781-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="4c781-113">Questo è il criterio che è stato restituito al passaggio 2.</span><span class="sxs-lookup"><span data-stu-id="4c781-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="4c781-114">Nella pagina regola di condivisione selezionare il livello di condivisione del calendario che si desidera consentire in **specificare le informazioni che si desidera condividere**. fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="4c781-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="4c781-115">Per ulteriori informazioni, vedere: ["il criterio non consente di concedere autorizzazioni a questo livello a uno o più destinatari" errore quando l'utente tenta di condividere il calendario](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="4c781-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
