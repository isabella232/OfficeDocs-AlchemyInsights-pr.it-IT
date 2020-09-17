---
title: Uso della prevenzione della perdita dei dati nelle regole di trasporto
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
- "9002635"
- "5153"
ms.openlocfilehash: 00ea5e67d1277e4a2a73d616b1f90d6e4bc5b54f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773167"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="0fd6b-102">Uso della prevenzione della perdita dei dati nelle regole di trasporto</span><span class="sxs-lookup"><span data-stu-id="0fd6b-102">Using DLP in transport rules</span></span>

<span data-ttu-id="0fd6b-103">Per integrare i criteri di prevenzione della perdita dei dati in un trasporto esistente, usare la condizione "**Se il messaggio contiene... informazioni riservate**" nell'impostazione della regola di trasporto.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="0fd6b-104">\*\*Per ulteriori dettagli, vedere \*\*.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-104">**For more details, see:**</span></span>

- <span data-ttu-id="0fd6b-105">Tipi di informazioni riservate per la prevenzione della perdita dei dati integrate nelle regole di trasporto: [Integrare le regole sulle informazioni riservate](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="0fd6b-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="0fd6b-106">È anche possibile testare la regola con o senza test dei criteri usando la modalità di test sulla regola.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="0fd6b-107">Attendere 30 minuti dopo la creazione della regola prima di eseguirne il test.</span><span class="sxs-lookup"><span data-stu-id="0fd6b-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="0fd6b-108">Vedere [Testare le regole del flusso di posta/di trasporto](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="0fd6b-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="0fd6b-109">**Nota**: se si sta cercando di implementare nuovi criteri di prevenzione della perdita dei dati con le regole di trasporto nell'interfaccia di amministrazione di Exchange, usare i [criteri di prevenzione della perdita dei dati nel Centro sicurezza e conformità](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="0fd6b-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
