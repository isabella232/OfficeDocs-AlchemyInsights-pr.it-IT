---
title: Leggere i registri di controllo per gli eventi eliminati
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464604"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="7c36c-102">Leggere i registri di controllo per gli eventi eliminati</span><span class="sxs-lookup"><span data-stu-id="7c36c-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="7c36c-103">Ecco come eseguire questa operazione:</span><span class="sxs-lookup"><span data-stu-id="7c36c-103">Here's how to do this:</span></span>

1. <span data-ttu-id="7c36c-104">Passare al Centro sicurezza e conformità di [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="7c36c-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="7c36c-105">Selezionare **Ricerca log** di  >  [**controllo**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="7c36c-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="7c36c-106">Se viene visualizzato un avviso che indica che è necessario attivare la funzionalità, procedere e attivarla ora.</span><span class="sxs-lookup"><span data-stu-id="7c36c-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="7c36c-107">Se la funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.</span><span class="sxs-lookup"><span data-stu-id="7c36c-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="7c36c-108">Selezionare **Attività** e quindi individuare le **attività della cassetta postale di Exchange.**</span><span class="sxs-lookup"><span data-stu-id="7c36c-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="7c36c-109">Selezionare le **opzioni Messaggi eliminati dalla cartella Posta** eliminata e Messaggi **spostati nella cartella** Posta eliminata.</span><span class="sxs-lookup"><span data-stu-id="7c36c-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="7c36c-110">Al termine, fare clic all'esterno del riquadro per ridurre a icona il **riquadro** Attività.</span><span class="sxs-lookup"><span data-stu-id="7c36c-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="7c36c-111">Specificare l'intervallo di date e quindi nella **casella** Utenti selezionare il nome utente per l'utente che si desidera analizzare.</span><span class="sxs-lookup"><span data-stu-id="7c36c-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="7c36c-112">È possibile selezionare più di un utente alla volta.</span><span class="sxs-lookup"><span data-stu-id="7c36c-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="7c36c-113">Selezionare **Cerca.**</span><span class="sxs-lookup"><span data-stu-id="7c36c-113">Select **Search**.</span></span> <span data-ttu-id="7c36c-114">Le attività vengono visualizzate in **Risultati.**</span><span class="sxs-lookup"><span data-stu-id="7c36c-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="7c36c-115">Per visualizzare i dettagli, selezionare un'attività e quindi **selezionare Altre informazioni.**</span><span class="sxs-lookup"><span data-stu-id="7c36c-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="7c36c-116">Ulteriori informazioni sull'elemento eliminato, ad esempio la riga dell'oggetto e la posizione dell'elemento al momento dell'eliminazione, vengono visualizzate nel campo **AffectedItems.**</span><span class="sxs-lookup"><span data-stu-id="7c36c-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="7c36c-117">Non è possibile ripristinare gli elementi eliminati utilizzando la funzionalità del log di controllo.</span><span class="sxs-lookup"><span data-stu-id="7c36c-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="7c36c-118">Per ripristinare gli elementi eliminati, vedere [Recuperare gli elementi eliminati o la posta elettronica in Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="7c36c-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="7c36c-119">Per ulteriori informazioni, vedere Eseguire una ricerca nel log di controllo di [Office 365 per risolvere i problemi relativi agli scenari comuni.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="7c36c-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
