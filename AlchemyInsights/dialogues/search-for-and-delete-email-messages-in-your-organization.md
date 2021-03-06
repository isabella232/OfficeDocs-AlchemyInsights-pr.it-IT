---
title: Cercare ed eliminare messaggi di posta elettronica nell'organizzazione
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500965"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="d4988-102">Cercare ed eliminare messaggi di posta elettronica nell'organizzazione</span><span class="sxs-lookup"><span data-stu-id="d4988-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="d4988-103">Eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="d4988-103">Follow these steps:</span></span>

1. <span data-ttu-id="d4988-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span><span class="sxs-lookup"><span data-stu-id="d4988-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="d4988-105">Per eliminare i messaggi, è necessario aggiungersi al gruppo di ruoli **Gestione** organizzazione o al ruolo di gestione Ricerca **ed eliminazione.**</span><span class="sxs-lookup"><span data-stu-id="d4988-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="d4988-106">Le autorizzazioni per questi ruoli vengono assegnate nel [Centro sicurezza & conformità.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="d4988-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="d4988-107">[Creare una ricerca di contenuto](https://docs.microsoft.com/office365/securitycompliance/content-search) per trovare il messaggio da eliminare.</span><span class="sxs-lookup"><span data-stu-id="d4988-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="d4988-108">[Connettersi a PowerShell in Centro sicurezza e conformità](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="d4988-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="d4988-109">Se si usa l'autenticazione a più fattori, vedere queste istruzioni: Connettersi a PowerShell & Centro sicurezza e [conformità con l'autenticazione a più fattori](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="d4988-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="d4988-110">Eliminare il messaggio: eseguire il `New-ComplianceSearchAction` cmdlet per eliminare il messaggio.</span><span class="sxs-lookup"><span data-stu-id="d4988-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="d4988-111">I messaggi eliminati vengono spostati nella cartella Elementi ripristinabili di un utente.</span><span class="sxs-lookup"><span data-stu-id="d4988-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="d4988-112">Per un comando di esempio, vedere [Passaggio 3: Eliminare il messaggio.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="d4988-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
