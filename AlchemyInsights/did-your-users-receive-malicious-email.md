---
title: Gli utenti hanno ricevuto messaggi pericolosi
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815250"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="774cf-102">Gli utenti hanno ricevuto messaggi pericolosi?</span><span class="sxs-lookup"><span data-stu-id="774cf-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="774cf-103">Ora è possibile segnalare il messaggio di posta elettronica dannoso a Microsoft attraverso gli [Invii degli amministratori nel Centro sicurezza e conformità](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="774cf-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="774cf-104">I messaggi segnalati negli [invii degli amministratori](https://sip.protection.office.com/reportsubmission) vengono analizzati e nel riquadro a comparsa **dettagli** vengono visualizzati i risultati seguenti:</span><span class="sxs-lookup"><span data-stu-id="774cf-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="774cf-105">Se si è verificato un errore nell'autenticazione della posta elettronica del mittente al momento del recapito.</span><span class="sxs-lookup"><span data-stu-id="774cf-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="774cf-106">Informazioni su eventuali riscontri dei criteri che potrebbero aver influenzato o sostituito il verdetto di un messaggio.</span><span class="sxs-lookup"><span data-stu-id="774cf-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="774cf-107">Risultati della detonazione correnti per verificare se gli URL o i file contenuti nel messaggio erano dannosi o meno.</span><span class="sxs-lookup"><span data-stu-id="774cf-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="774cf-108">Feedback da parte di valutatori</span><span class="sxs-lookup"><span data-stu-id="774cf-108">Feedback from graders</span></span>

<span data-ttu-id="774cf-109">Se è stata trovata una sostituzione, la nuova analisi dovrebbe essere completata dopo alcuni minuti.</span><span class="sxs-lookup"><span data-stu-id="774cf-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="774cf-110">Se non si è verificato un problema nell'autenticazione della posta elettronica o il recapito non è stato influenzato da una sostituzione, per il feedback da parte dei valutatori potrebbe essere necessario fino a un giorno.</span><span class="sxs-lookup"><span data-stu-id="774cf-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="774cf-111">Se non si è d'accordo con il risultato finale su un messaggio, un URL o un file (bloccato o non bloccato), inviare di nuovo il messaggio dopo un giorno per ripetere l'analisi.</span><span class="sxs-lookup"><span data-stu-id="774cf-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="774cf-112">È molto probabile che il verdetto cambi dopo aver inviato di nuovo il messaggio.</span><span class="sxs-lookup"><span data-stu-id="774cf-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="774cf-113">Nel frattempo, è possibile rimuovere il messaggio di posta elettronica dannoso dalla casella di Posta in arrivo dell'utente seguendo le istruzioni in [questo articolo](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="774cf-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="774cf-114">I clienti che hanno Microsoft Defender per Office 365 possono:</span><span class="sxs-lookup"><span data-stu-id="774cf-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="774cf-115">usare [Esplora minacce per trovare ed eliminare i messaggi sospetti](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="774cf-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="774cf-116">[usare i collegamenti sicuri per bloccare l'accesso](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) a un URL dannoso</span><span class="sxs-lookup"><span data-stu-id="774cf-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="774cf-117">tenere traccia degli utenti che hanno fatto clic ed eseguito l'accesso a URL dannosi: [Visualizzare l'URL di phishing e fare clic sui dati del verdetto](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-Url Track](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="774cf-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="774cf-118">[avviare manualmente una indagine automatizzata](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="774cf-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="774cf-119">Ci si può proteggere da file e URL dannosi anche seguendo le istruzioni fornite in [Protezione da URL e file dannosi](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="774cf-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>