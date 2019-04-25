---
title: 1332 OWA-la regola di posta in arrivo non è in esecuzione per una cassetta postale
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372564"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="b2997-102">Una regola di posta in arrivo non funziona come previsto</span><span class="sxs-lookup"><span data-stu-id="b2997-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="b2997-103">Verificare le impostazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="b2997-103">Verify the following settings:</span></span>

- <span data-ttu-id="b2997-104">Un messaggio può essere reindirizzato, inoltrato o risposto automaticamente in base alle regole della posta in arrivo solo una volta.</span><span class="sxs-lookup"><span data-stu-id="b2997-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="b2997-105">Una regola di reindirizzamento (una regola di posta in arrivo o una regola del flusso di posta, nota anche come regola di trasporto) può aggiungere un massimo di dieci destinatari di inoltro a un messaggio.</span><span class="sxs-lookup"><span data-stu-id="b2997-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="b2997-106">Per ulteriori informazioni, vedere [Journal, Transport, and Inbox Rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="b2997-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="b2997-107">Le regole di posta in arrivo non funzionano nella cassetta postale di inserimento nel journal alternativa.</span><span class="sxs-lookup"><span data-stu-id="b2997-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="b2997-108">Per ulteriori informazioni sulla cassetta postale di inserimento nel journal alternativa, vedere [cassetta del journalIng alternativa](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="b2997-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="b2997-109">Per risolvere questi problemi, vedere [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="b2997-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="b2997-110">Se non si applicano i problemi precedenti, eseguire il rapporto di diagnostica della regola di posta in arrivo prima di inoltrare il problema al supporto tecnico Microsoft:</span><span class="sxs-lookup"><span data-stu-id="b2997-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="b2997-111">Aprire la cassetta postale in Outlook sul Web e fare clic su **Opzioni** \> **Impostazioni** \> per **organizzare** \> **le regole**della posta in arrivo.</span><span class="sxs-lookup"><span data-stu-id="b2997-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="b2997-112">Nella parte inferiore della pagina fare clic su **se le regole non funzionano, fare clic qui per generare un rapporto di diagnostica**.</span><span class="sxs-lookup"><span data-stu-id="b2997-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
