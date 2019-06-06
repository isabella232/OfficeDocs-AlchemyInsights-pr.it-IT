---
title: Introduzione a SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: a44b2c7b26895e09c24df772f1ada9a2e3483747
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735987"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="dcfe3-102">Flussi di lavoro in SharePoint</span><span class="sxs-lookup"><span data-stu-id="dcfe3-102">Workflows in SharePoint</span></span>

<span data-ttu-id="dcfe3-103">Se i flussi di lavoro di SharePoint non inviano messaggi di posta elettronica, è possibile che l'organizzazione abbia incontrato i limiti dei mittenti di Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="dcfe3-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="dcfe3-104">Il messaggio di errore "flusso di lavoro è sospeso" può verificarsi se si dispone di uno degli elementi seguenti:</span><span class="sxs-lookup"><span data-stu-id="dcfe3-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="dcfe3-105">Si dispone di un flusso di lavoro in SharePoint Online che utilizza il tipo di piattaforma per flussi di lavoro di SharePoint 2010 o SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="dcfe3-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="dcfe3-106">Il flusso di lavoro è configurato per inviare un messaggio di posta elettronica personalizzato a più di 200 utenti alla volta, più di 10.000 destinatari al giorno o più di 30 messaggi al minuto.</span><span class="sxs-lookup"><span data-stu-id="dcfe3-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="dcfe3-107">Quando si esegue il flusso di lavoro, il messaggio di posta elettronica non viene inviato e si nota il messaggio di errore, lo stato interno è impostato su sospeso o non è in grado di inviare a un destinatario viene visualizzato.</span><span class="sxs-lookup"><span data-stu-id="dcfe3-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="dcfe3-108">Per ulteriori informazioni, vedere l' [articolo](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US)seguente.</span><span class="sxs-lookup"><span data-stu-id="dcfe3-108">For more information, please refer to the following [article](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

