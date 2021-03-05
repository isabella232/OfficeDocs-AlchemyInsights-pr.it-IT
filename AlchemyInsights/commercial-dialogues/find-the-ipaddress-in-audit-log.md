---
title: Trovare l'indirizzo IP nel registro di controllo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465002"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="7b2f1-102">Trovare l'indirizzo IP nel registro di controllo</span><span class="sxs-lookup"><span data-stu-id="7b2f1-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="7b2f1-103">L'indirizzo IP corrispondente a un'attività eseguita da un utente o da un amministratore viene visualizzato nei registri di controllo.</span><span class="sxs-lookup"><span data-stu-id="7b2f1-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="7b2f1-104">Vengono registrate anche le informazioni sul client.</span><span class="sxs-lookup"><span data-stu-id="7b2f1-104">The client information is also logged.</span></span> <span data-ttu-id="7b2f1-105">Ecco come identificare l'indirizzo IP:</span><span class="sxs-lookup"><span data-stu-id="7b2f1-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="7b2f1-106">Passare al Centro sicurezza e conformità di [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="7b2f1-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="7b2f1-107">Selezionare **Ricerca log** di  >  **[controllo](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="7b2f1-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="7b2f1-108">Se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora.</span><span class="sxs-lookup"><span data-stu-id="7b2f1-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="7b2f1-109">Se questa funzionalità non è abilitata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.</span><span class="sxs-lookup"><span data-stu-id="7b2f1-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="7b2f1-110">Se sei interessato a un'attività specifica, selezionala **nell'elenco** Attività. In caso contrario, per impostazione predefinita verranno restituite tutte le attività per l'utente selezionato.</span><span class="sxs-lookup"><span data-stu-id="7b2f1-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="7b2f1-111">Si noti che alcune attività potrebbero non essere disponibili per la selezione **dal** menu Attività. Tuttavia, tali elementi di controllo verranno restituiti se **è selezionata l'opzione** Mostra risultati per tutte le attività (impostazione predefinita).</span><span class="sxs-lookup"><span data-stu-id="7b2f1-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="7b2f1-112">Specificare l'intervallo di date e nel **campo Utenti** selezionare il nome utente dell'utente che si desidera analizzare.</span><span class="sxs-lookup"><span data-stu-id="7b2f1-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="7b2f1-113">Selezionare **Cerca.**</span><span class="sxs-lookup"><span data-stu-id="7b2f1-113">Select **Search**.</span></span> <span data-ttu-id="7b2f1-114">Le attività vengono visualizzate in **Risultati.**</span><span class="sxs-lookup"><span data-stu-id="7b2f1-114">The activities appear under **Results**.</span></span> <span data-ttu-id="7b2f1-115">È possibile visualizzare l'indirizzo IP per ogni attività.</span><span class="sxs-lookup"><span data-stu-id="7b2f1-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="7b2f1-116">Per visualizzare i dettagli, selezionare un'attività e quindi **selezionare Altre informazioni.**</span><span class="sxs-lookup"><span data-stu-id="7b2f1-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="7b2f1-117">Per ulteriori informazioni, vedere Eseguire una ricerca nel log di controllo di [Office 365 per risolvere i problemi relativi agli scenari comuni.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="7b2f1-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>