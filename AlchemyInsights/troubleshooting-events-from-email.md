---
title: Risoluzione dei problemi relativi agli eventi da posta elettronica
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834843"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="a70c1-102">Risoluzione dei problemi relativi agli eventi da posta elettronica</span><span class="sxs-lookup"><span data-stu-id="a70c1-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="a70c1-103">Verificare che la funzionalità sia abilitata per la cassetta postale: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="a70c1-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="a70c1-104">Osservare quindi i log "Eventi da posta elettronica" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="a70c1-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="a70c1-105">Nei log casella "Eventi da posta elettronica" trovare il valore InternetMessageId che corrisponde all'elemento nella cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="a70c1-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="a70c1-106">Il valore TrustScore determina se l'elemento viene aggiunto o meno.</span><span class="sxs-lookup"><span data-stu-id="a70c1-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="a70c1-107">Gli eventi verranno aggiunti solo se TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="a70c1-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="a70c1-108">Il valore TrustScore è determinata dalle proprietà SPF, DKIM o DMARC, che si trovano nell'intestazione del messaggio.</span><span class="sxs-lookup"><span data-stu-id="a70c1-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="a70c1-109">Per visualizzare queste proprietà:</span><span class="sxs-lookup"><span data-stu-id="a70c1-109">To view these properties:</span></span>

<span data-ttu-id="a70c1-110">**Outlook desktop**</span><span class="sxs-lookup"><span data-stu-id="a70c1-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="a70c1-111">Aprire l'elemento</span><span class="sxs-lookup"><span data-stu-id="a70c1-111">Open the item</span></span>
- <span data-ttu-id="a70c1-112">File -> Proprietà -> Intestazioni Internet</span><span class="sxs-lookup"><span data-stu-id="a70c1-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="a70c1-113">oppure</span><span class="sxs-lookup"><span data-stu-id="a70c1-113">or</span></span>

<span data-ttu-id="a70c1-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="a70c1-114">**MFCMapi**</span></span>

- <span data-ttu-id="a70c1-115">Passare all'elemento nella cartella di posta in arrivo</span><span class="sxs-lookup"><span data-stu-id="a70c1-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="a70c1-116">Cercare PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="a70c1-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="a70c1-117">Queste proprietà sono determinate e registrate durante il trasporto e il routing.</span><span class="sxs-lookup"><span data-stu-id="a70c1-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="a70c1-118">Per altre informazioni sulla risoluzione dei problemi, potrebbe essere necessario continuare con il supporto del trasporto per i problemi in SPF, DKIM e DMARC.</span><span class="sxs-lookup"><span data-stu-id="a70c1-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>