---
title: Identificare l'indirizzo IP e il client nei registri di controllo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668314"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="fbcad-102">Identificare l'indirizzo IP e il client nei registri di controllo</span><span class="sxs-lookup"><span data-stu-id="fbcad-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="fbcad-103">L'indirizzo IP che corrisponde a un'attività di un utente o di un amministratore di Microsoft 365 viene visualizzato nei registri di controllo.</span><span class="sxs-lookup"><span data-stu-id="fbcad-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="fbcad-104">Vengono inoltre registrate le informazioni sul client.</span><span class="sxs-lookup"><span data-stu-id="fbcad-104">The client information is also logged.</span></span> <span data-ttu-id="fbcad-105">Di seguito vengono illustrati i passaggi per identificare tali informazioni</span><span class="sxs-lookup"><span data-stu-id="fbcad-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="fbcad-106">Accedere al [Centro sicurezza & conformità di Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="fbcad-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="fbcad-107">Passare alla pagina di ricerca del registro di controllo della **ricerca**  >  **Audit log search** .</span><span class="sxs-lookup"><span data-stu-id="fbcad-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="fbcad-108">Se si è interessati a un'attività specifica, selezionarla dall'elenco **attività** .</span><span class="sxs-lookup"><span data-stu-id="fbcad-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="fbcad-109">In caso contrario, verranno restituite tutte le attività per l'utente selezionato (impostazione predefinita).</span><span class="sxs-lookup"><span data-stu-id="fbcad-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="fbcad-110">**Nota**: alcune attività potrebbero non essere disponibili nel menu **attività** ; Tuttavia, tali elementi di controllo verranno restituiti se è selezionata l'opzione **Mostra risultati per tutte le attività** (impostazione predefinita).</span><span class="sxs-lookup"><span data-stu-id="fbcad-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="fbcad-111">Specificare il nome utente nel campo **utenti** , selezionare l'intervallo di date appropriato per l'attività, quindi fare clic su **Cerca**.</span><span class="sxs-lookup"><span data-stu-id="fbcad-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="fbcad-112">Nei risultati, è possibile visualizzare l'indirizzo IP per tale attività nel riquadro dei risultati.</span><span class="sxs-lookup"><span data-stu-id="fbcad-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="fbcad-113">Selezionare il record di controllo per visualizzare informazioni dettagliate nel riquadro a comparsa dei **Dettagli** , ad esempio client, utente che ha eseguito un'azione e così via.</span><span class="sxs-lookup"><span data-stu-id="fbcad-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="fbcad-114">Per ulteriori informazioni, vedere [trovare l'indirizzo IP del computer utilizzato per accedere a un account compromesso](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="fbcad-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
