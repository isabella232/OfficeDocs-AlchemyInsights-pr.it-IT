---
title: Scoprire chi ha configurato l'inoltro su una cassetta postale e come
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464616"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="15185-102">Scoprire chi ha configurato l'inoltro su una cassetta postale e come</span><span class="sxs-lookup"><span data-stu-id="15185-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="15185-103">Se l'inoltro esterno è stato impostato su una cassetta postale, l'attività viene verificata come parte del cmdlet Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="15185-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="15185-104">Ecco come trovare l'attività nel log di controllo:</span><span class="sxs-lookup"><span data-stu-id="15185-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="15185-105">Passare al Centro sicurezza e conformità di [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="15185-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="15185-106">Selezionare **Ricerca log** di >  **controllo**.</span><span class="sxs-lookup"><span data-stu-id="15185-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="15185-107">Se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora.</span><span class="sxs-lookup"><span data-stu-id="15185-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="15185-108">Se questa funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.</span><span class="sxs-lookup"><span data-stu-id="15185-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="15185-109">Verificare che il **campo Attività** sia impostato su Mostra risultati per tutte **le attività** (impostazione predefinita).</span><span class="sxs-lookup"><span data-stu-id="15185-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="15185-110">Specificare l'intervallo di date.</span><span class="sxs-lookup"><span data-stu-id="15185-110">Specify the date range.</span></span> <span data-ttu-id="15185-111">Non è necessario specificare un nome utente.</span><span class="sxs-lookup"><span data-stu-id="15185-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="15185-112">Selezionare **Cerca.**</span><span class="sxs-lookup"><span data-stu-id="15185-112">Select **Search**.</span></span> <span data-ttu-id="15185-113">Le attività vengono visualizzate in **Risultati.**</span><span class="sxs-lookup"><span data-stu-id="15185-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="15185-114">Selezionare **Risultati filtro,** quindi immettere **Set-mailbox** nel **campo Filtro** attività.</span><span class="sxs-lookup"><span data-stu-id="15185-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="15185-115">In questo modo vengono **restituite tutte le attività Set-Mailbox.**</span><span class="sxs-lookup"><span data-stu-id="15185-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="15185-116">Per visualizzare i dettagli, selezionare un'attività e quindi **selezionare Altre informazioni.**</span><span class="sxs-lookup"><span data-stu-id="15185-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="15185-117">In **Parametri** è possibile visualizzare l'indirizzo di posta elettronica di inoltro impostato nella cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="15185-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="15185-118">**L'ID utente** rappresenta l'utente che ha configurato l'inoltro esterno nella cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="15185-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="15185-119">Per ulteriori informazioni, vedere Eseguire una ricerca nel log di controllo di [Office 365 per risolvere i problemi relativi agli scenari comuni.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="15185-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>