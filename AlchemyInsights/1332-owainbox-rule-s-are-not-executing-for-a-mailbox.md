---
title: 1332 OWA - regole posta in arrivo non vengono eseguiti per una cassetta postale
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915808"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="0c678-102">Una regola di posta in arrivo non funziona come previsto</span><span class="sxs-lookup"><span data-stu-id="0c678-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="0c678-103">Verificare le impostazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="0c678-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="0c678-p101">Un messaggio può essere reindirizzato, inoltrato o di risposta per automaticamente in base alle regole posta in arrivo una sola volta. Una regola di reindirizzare la chiamata (una regola di posta in arrivo o una regola del flusso di posta, noto anche come una regola di trasporto) è possibile aggiungere un massimo di dieci destinatari inoltro a un messaggio. Per ulteriori informazioni, vedere [limiti delle regole del Journal, trasporto e posta in arrivo](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="0c678-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="0c678-p102">Regole posta in arrivo non funzionano con la cassetta del journaling alternativa. Per ulteriori informazioni sulla cassetta del journaling alternativo, vedere [cassetta del journaling alternativa](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="0c678-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="0c678-109">Per risolvere questi problemi, vedere [2829319 KB](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="0c678-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="0c678-110">Se non si applicano i problemi precedenti, eseguire il rapporto di diagnostica regola posta in arrivo prima trasformare il problema al supporto Microsoft:</span><span class="sxs-lookup"><span data-stu-id="0c678-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="0c678-111">Aprire la cassetta postale di Outlook sul web e fare clic su **Impostazioni** \> **Opzioni** \> **Organizza posta** \> **regole posta in arrivo**.</span><span class="sxs-lookup"><span data-stu-id="0c678-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="0c678-112">Nella parte inferiore della pagina, fare clic su **se le regole non funzionano fare clic qui per generare un rapporto di diagnostica**.</span><span class="sxs-lookup"><span data-stu-id="0c678-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

