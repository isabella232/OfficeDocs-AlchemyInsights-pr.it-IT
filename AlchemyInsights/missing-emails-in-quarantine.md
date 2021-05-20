---
title: Messaggi di posta elettronica mancanti in quarantena
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539828"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="00819-102">Messaggi di posta elettronica mancanti in quarantena"</span><span class="sxs-lookup"><span data-stu-id="00819-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="00819-103">Gli amministratori [possono visualizzare, rilasciare o eliminare questi messaggi.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="00819-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="00819-104">Per aprire il Centro sicurezza & conformità, passare a [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="00819-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="00819-105">Per aprire direttamente la pagina Quarantena, passare a [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="00819-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="00819-106">È possibile cercare in base ai seguenti valori:</span><span class="sxs-lookup"><span data-stu-id="00819-106">You can search by the following values:</span></span>  

- <span data-ttu-id="00819-107">**ID messaggio**: identificatore univoco globale del messaggio.</span><span class="sxs-lookup"><span data-stu-id="00819-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="00819-108">Se si seleziona un messaggio nell'elenco, il valore  **ID**  messaggio verrà visualizzato  **nel**  riquadro a comparsa Dettagli visualizzato.</span><span class="sxs-lookup"><span data-stu-id="00819-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="00819-109">Gli amministratori possono usare [Traccia messaggio](/microsoft-365/security/office-365-security/message-trace-scc) per trovare i messaggi e i valori ID messaggio corrispondenti.</span><span class="sxs-lookup"><span data-stu-id="00819-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="00819-110">**Indirizzo di posta elettronica del mittente**: indirizzo di posta elettronica di un singolo mittente.</span><span class="sxs-lookup"><span data-stu-id="00819-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="00819-111">**Indirizzo di posta elettronica del destinatario**: indirizzo di posta elettronica di un singolo destinatario.</span><span class="sxs-lookup"><span data-stu-id="00819-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="00819-112">**Oggetto**: utilizzare l'intero oggetto del messaggio.</span><span class="sxs-lookup"><span data-stu-id="00819-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="00819-113">Per la ricerca non viene fatta distinzione tra maiuscole e minuscole.</span><span class="sxs-lookup"><span data-stu-id="00819-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="00819-114">Dopo avere immesso i criteri di ricerca, fare clic sul ![pulsante Aggiorna](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Aggiorna** per filtrare i risultati.</span><span class="sxs-lookup"><span data-stu-id="00819-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="00819-115">I cmdlet utilizzati per visualizzare e gestire i messaggi e i file in quarantena sono:</span><span class="sxs-lookup"><span data-stu-id="00819-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="00819-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="00819-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="00819-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="00819-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="00819-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="00819-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="00819-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): questo cmdlet è valido solo per i messaggi e non per i file di malware di Microsoft Defender per Office 365 per SharePoint Online, OneDrive for Business o Teams.</span><span class="sxs-lookup"><span data-stu-id="00819-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="00819-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="00819-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)