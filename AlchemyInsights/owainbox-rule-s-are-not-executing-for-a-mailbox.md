---
title: 1332 OWA-la regola di posta in arrivo non è in esecuzione per una cassetta postale
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576564"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="61cf6-102">Una regola di posta in arrivo non funziona come previsto</span><span class="sxs-lookup"><span data-stu-id="61cf6-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="61cf6-103">Verificare le impostazioni seguenti in Outlook sul Web:</span><span class="sxs-lookup"><span data-stu-id="61cf6-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="61cf6-104">Un messaggio può essere reindirizzato, inoltrato o risposto automaticamente in base alle regole della posta in arrivo solo una volta.</span><span class="sxs-lookup"><span data-stu-id="61cf6-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="61cf6-105">Una regola di reindirizzamento (una regola di posta in arrivo o una regola del flusso di posta, nota anche come regola di trasporto) può aggiungere un massimo di dieci destinatari di inoltro a un messaggio.</span><span class="sxs-lookup"><span data-stu-id="61cf6-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="61cf6-106">Per ulteriori informazioni, vedere [Journal, Transport, and Inbox Rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="61cf6-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="61cf6-107">Le regole di posta in arrivo non funzionano nella cassetta postale di inserimento nel journal alternativa.</span><span class="sxs-lookup"><span data-stu-id="61cf6-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="61cf6-108">Per ulteriori informazioni sulla cassetta postale di inserimento nel journal alternativa, vedere [cassetta del journaling alternativa](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="61cf6-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="61cf6-109">Per risolvere questi problemi, vedere [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="61cf6-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="61cf6-110">Se non si applicano i problemi precedenti, eseguire il rapporto di diagnostica della regola di posta in arrivo prima di inoltrare il problema al supporto tecnico Microsoft:</span><span class="sxs-lookup"><span data-stu-id="61cf6-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="61cf6-111">Aprire la cassetta postale in Outlook sul Web e fare clic su</span><span class="sxs-lookup"><span data-stu-id="61cf6-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="61cf6-112">**Impostazioni**  >  di **Visualizzazione di tutte le impostazioni**  >  di Outlook **Posta elettronica**  >  **Regole**.</span><span class="sxs-lookup"><span data-stu-id="61cf6-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="61cf6-113">Nella parte inferiore della pagina fare clic su **se le regole non funzionano, fare clic qui per generare un rapporto di diagnostica**.</span><span class="sxs-lookup"><span data-stu-id="61cf6-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
