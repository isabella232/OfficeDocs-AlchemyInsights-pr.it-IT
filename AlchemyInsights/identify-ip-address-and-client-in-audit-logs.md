---
title: Identificare l'indirizzo IP e il client nei registri di controllo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752064"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="879ab-102">Identificare l'indirizzo IP e il client nei registri di controllo</span><span class="sxs-lookup"><span data-stu-id="879ab-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="879ab-103">L'indirizzo IP corrispondente a un'attività di un utente o di un amministratore viene visualizzato nei registri di controllo.</span><span class="sxs-lookup"><span data-stu-id="879ab-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="879ab-104">Vengono inoltre registrate le informazioni sul client.</span><span class="sxs-lookup"><span data-stu-id="879ab-104">The client information is also logged.</span></span> <span data-ttu-id="879ab-105">Di seguito vengono illustrati i passaggi per identificare tali informazioni</span><span class="sxs-lookup"><span data-stu-id="879ab-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="879ab-106">Accedere al [Centro sicurezza & conformità di Office 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="879ab-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="879ab-107">Fare clic su **ricerca e analisi** e selezionare **Ricerca log di controllo**.</span><span class="sxs-lookup"><span data-stu-id="879ab-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="879ab-108">Se si è interessati a un'attività specifica, selezionarla dall'elenco **attività** .</span><span class="sxs-lookup"><span data-stu-id="879ab-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="879ab-109">In caso contrario, verranno restituite tutte le attività per l'utente selezionato (impostazione predefinita).</span><span class="sxs-lookup"><span data-stu-id="879ab-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="879ab-110">**Nota**: alcune attività potrebbero non essere disponibili nel menu **attività** ; Tuttavia, tali elementi di controllo verranno restituiti se è selezionata l'opzione **Mostra risultati per tutte le attività** (impostazione predefinita).</span><span class="sxs-lookup"><span data-stu-id="879ab-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="879ab-111">Specificare il nome utente nel campo **utenti** , selezionare l'intervallo di date appropriato per l'attività, quindi fare clic su **Cerca**.</span><span class="sxs-lookup"><span data-stu-id="879ab-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="879ab-112">Nei risultati, è possibile visualizzare l'indirizzo IP per tale attività nel riquadro dei risultati.</span><span class="sxs-lookup"><span data-stu-id="879ab-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="879ab-113">Selezionare il record di controllo per visualizzare informazioni dettagliate nel riquadro a comparsa dei **Dettagli** , ad esempio client, utente che ha eseguito un'azione e così via.</span><span class="sxs-lookup"><span data-stu-id="879ab-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="879ab-114">Per ulteriori informazioni, vedere [trovare l'indirizzo IP del computer utilizzato per accedere a un account compromesso](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="879ab-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
