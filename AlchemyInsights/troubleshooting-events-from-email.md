---
title: Risoluzione dei problemi relativi agli eventi da posta elettronica
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658738"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="2f210-102">Risoluzione dei problemi relativi agli eventi da posta elettronica</span><span class="sxs-lookup"><span data-stu-id="2f210-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="2f210-103">Verificare che la funzionalità sia abilitata per la cassetta postale: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="2f210-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="2f210-104">Osservare quindi i log "Eventi da posta elettronica" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="2f210-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="2f210-105">Nei log casella "Eventi da posta elettronica" trovare il valore InternetMessageId che corrisponde all'elemento nella cassetta postale.</span><span class="sxs-lookup"><span data-stu-id="2f210-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="2f210-106">Il valore TrustScore determina se l'elemento viene aggiunto o meno.</span><span class="sxs-lookup"><span data-stu-id="2f210-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="2f210-107">Gli eventi verranno aggiunti solo se TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="2f210-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="2f210-108">Il valore TrustScore è determinata dalle proprietà SPF, DKIM o DMARC, che si trovano nell'intestazione del messaggio.</span><span class="sxs-lookup"><span data-stu-id="2f210-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="2f210-109">Per visualizzare queste proprietà:</span><span class="sxs-lookup"><span data-stu-id="2f210-109">To view these properties:</span></span>

<span data-ttu-id="2f210-110">**Outlook desktop**</span><span class="sxs-lookup"><span data-stu-id="2f210-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="2f210-111">Aprire l'elemento</span><span class="sxs-lookup"><span data-stu-id="2f210-111">Open the item</span></span>
- <span data-ttu-id="2f210-112">File -> Proprietà -> Intestazioni Internet</span><span class="sxs-lookup"><span data-stu-id="2f210-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="2f210-113">oppure</span><span class="sxs-lookup"><span data-stu-id="2f210-113">or</span></span>

<span data-ttu-id="2f210-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="2f210-114">**MFCMapi**</span></span>

- <span data-ttu-id="2f210-115">Passare all'elemento nella cartella di posta in arrivo</span><span class="sxs-lookup"><span data-stu-id="2f210-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="2f210-116">Cercare PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="2f210-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="2f210-117">Queste proprietà sono determinate e registrate durante il trasporto e il routing.</span><span class="sxs-lookup"><span data-stu-id="2f210-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="2f210-118">Per altre informazioni sulla risoluzione dei problemi, potrebbe essere necessario continuare con il supporto del trasporto per i problemi in SPF, DKIM e DMARC.</span><span class="sxs-lookup"><span data-stu-id="2f210-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>