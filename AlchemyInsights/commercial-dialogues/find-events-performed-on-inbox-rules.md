---
title: Trovare gli eventi eseguiti sulle regole di Posta in arrivo
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465001"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="18ea7-102">Trovare gli eventi eseguiti sulle regole di Posta in arrivo</span><span class="sxs-lookup"><span data-stu-id="18ea7-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="18ea7-103">Quando le regole di Posta in arrivo vengono create, modificate o eliminate, gli eventi vengono registrati nel registro di controllo.</span><span class="sxs-lookup"><span data-stu-id="18ea7-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="18ea7-104">Ecco come esaminarli:</span><span class="sxs-lookup"><span data-stu-id="18ea7-104">Here's how to review them:</span></span>

1. <span data-ttu-id="18ea7-105">Passare al Centro sicurezza e conformità di [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="18ea7-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="18ea7-106">Selezionare Ricerca > ricerca nel log di controllo.</span><span class="sxs-lookup"><span data-stu-id="18ea7-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="18ea7-107">Se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora.</span><span class="sxs-lookup"><span data-stu-id="18ea7-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="18ea7-108">Se questa funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.</span><span class="sxs-lookup"><span data-stu-id="18ea7-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="18ea7-109">Selezionare il campo Attività e trovare le attività della cassetta postale di Exchange, quindi selezionare New-InboxRule Crea regola posta in arrivo da Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="18ea7-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="18ea7-110">Al termine, fare clic all'esterno del riquadro per ridurre a icona il riquadro Attività.</span><span class="sxs-lookup"><span data-stu-id="18ea7-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="18ea7-111">Specificare l'intervallo di date e quindi nel campo Utenti selezionare il nome utente per l'utente che si desidera analizzare.</span><span class="sxs-lookup"><span data-stu-id="18ea7-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="18ea7-112">È possibile selezionare più di un utente alla volta.</span><span class="sxs-lookup"><span data-stu-id="18ea7-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="18ea7-113">Selezionare Cerca.</span><span class="sxs-lookup"><span data-stu-id="18ea7-113">Select Search.</span></span> <span data-ttu-id="18ea7-114">Le attività vengono visualizzate in Risultati.</span><span class="sxs-lookup"><span data-stu-id="18ea7-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="18ea7-115">Per visualizzare i dettagli, selezionare un'attività e quindi selezionare Altre informazioni.</span><span class="sxs-lookup"><span data-stu-id="18ea7-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="18ea7-116">Nella sezione Parametri è possibile visualizzare il nome della regola, le condizioni impostate e le azioni che verranno eseguite dalla regola.</span><span class="sxs-lookup"><span data-stu-id="18ea7-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="18ea7-117">Per ulteriori informazioni, vedere Eseguire una ricerca nel log di controllo di Office 365 per risolvere i problemi relativi agli scenari comuni.</span><span class="sxs-lookup"><span data-stu-id="18ea7-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>