---
title: Superamento del limite di posta elettronica giornaliero. Il flusso di lavoro è sospeso.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514461"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="bf04d-103">Superamento del limite di posta elettronica giornaliero.</span><span class="sxs-lookup"><span data-stu-id="bf04d-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="bf04d-104">Il flusso di lavoro è sospeso.</span><span class="sxs-lookup"><span data-stu-id="bf04d-104">Workflow is suspended.</span></span>

<span data-ttu-id="bf04d-105">Questo errore può essere ricevuto negli scenari seguenti:</span><span class="sxs-lookup"><span data-stu-id="bf04d-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="bf04d-106">Si dispone di un flusso di lavoro in SharePoint Online che utilizza il tipo di piattaforma per flussi di lavoro di SharePoint 2010 o SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="bf04d-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="bf04d-107">Il flusso di lavoro è configurato per inviare un messaggio di posta elettronica personalizzato a più di 200 utenti alla volta, più di 10.000 destinatari al giorno o più di 30 messaggi al minuto.</span><span class="sxs-lookup"><span data-stu-id="bf04d-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="bf04d-108">Quando si esegue il flusso di lavoro, il messaggio di posta elettronica non viene inviato e si nota il comportamento seguente:</span><span class="sxs-lookup"><span data-stu-id="bf04d-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="bf04d-109">Per un flusso di lavoro che utilizza il tipo di piattaforma SharePoint 2013, passare alla pagina **stato flusso di lavoro** .</span><span class="sxs-lookup"><span data-stu-id="bf04d-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="bf04d-110">Nella pagina Stato flusso di lavoro lo **stato interno** è impostato su **avviato**e il fumetto di informazioni non è in **grado di inviare messaggi a un destinatario**.</span><span class="sxs-lookup"><span data-stu-id="bf04d-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="bf04d-111">Per ovviare a questo problema, configurare il flusso di lavoro per l'invio di messaggi di posta elettronica senza superare i [limiti dei mittenti di Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="bf04d-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="bf04d-112">Ad esempio, utilizzare una pausa nel flusso di lavoro, inviare il messaggio di posta elettronica a un gruppo di Office 365, a un gruppo di distribuzione o di sicurezza abilitato alla posta elettronica oppure inviare i messaggi a un numero di destinatari inferiore a 200 alla volta.</span><span class="sxs-lookup"><span data-stu-id="bf04d-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="bf04d-113">Per ulteriori informazioni, vedere l' [articolo](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)seguente.</span><span class="sxs-lookup"><span data-stu-id="bf04d-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="bf04d-114">Argomenti correlati</span><span class="sxs-lookup"><span data-stu-id="bf04d-114">Related topics</span></span>
- [<span data-ttu-id="bf04d-115">Crea flusso</span><span class="sxs-lookup"><span data-stu-id="bf04d-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="bf04d-116">SharePoint e flusso</span><span class="sxs-lookup"><span data-stu-id="bf04d-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 