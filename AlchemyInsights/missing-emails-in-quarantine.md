---
title: Messaggi di posta elettronica mancanti in quarantena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542153"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="314b7-102">Messaggi di posta elettronica mancanti in quarantena "</span><span class="sxs-lookup"><span data-stu-id="314b7-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="314b7-103">Gli amministratori possono [visualizzare, rilasciare o eliminare questi messaggi.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="314b7-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="314b7-104">Per aprire il Centro sicurezza & conformità, accedere a [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="314b7-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="314b7-105">Per aprire direttamente la pagina di quarantena, andare a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="314b7-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="314b7-106">È possibile cercare in base ai seguenti valori:</span><span class="sxs-lookup"><span data-stu-id="314b7-106">You can search by the following values:</span></span>  

- <span data-ttu-id="314b7-107">**ID messaggio**: identificatore univoco globale del messaggio.</span><span class="sxs-lookup"><span data-stu-id="314b7-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="314b7-108">Se si seleziona un messaggio nell'elenco, il valore **ID messaggio** verrà visualizzato nel riquadro a comparsa **Dettagli** visualizzato.</span><span class="sxs-lookup"><span data-stu-id="314b7-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="314b7-109">Gli amministratori possono usare [Traccia messaggio](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) per trovare i messaggi e i valori ID messaggio corrispondenti.</span><span class="sxs-lookup"><span data-stu-id="314b7-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="314b7-110">**Indirizzo di posta elettronica del mittente**: indirizzo di posta elettronica di un singolo mittente.</span><span class="sxs-lookup"><span data-stu-id="314b7-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="314b7-111">**Indirizzo di posta elettronica del destinatario**: indirizzo di posta elettronica di un singolo destinatario.</span><span class="sxs-lookup"><span data-stu-id="314b7-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="314b7-112">**Oggetto**: utilizzare l'intero oggetto del messaggio.</span><span class="sxs-lookup"><span data-stu-id="314b7-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="314b7-113">Per la ricerca non viene fatta distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="314b7-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="314b7-114">Dopo aver immesso i criteri di ricerca, fare clic su Aggiorna ![ pulsante ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** di aggiornamento per filtrare i risultati.  </span><span class="sxs-lookup"><span data-stu-id="314b7-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="314b7-115">I cmdlet utilizzati per visualizzare e gestire i messaggi e i file in quarantena sono i seguenti:</span><span class="sxs-lookup"><span data-stu-id="314b7-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="314b7-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="314b7-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="314b7-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="314b7-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="314b7-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="314b7-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="314b7-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): si noti che questo cmdlet è solo per i messaggi, non per i file malware da ATP per SharePoint Online, OneDrive for business o teams.</span><span class="sxs-lookup"><span data-stu-id="314b7-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="314b7-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="314b7-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)