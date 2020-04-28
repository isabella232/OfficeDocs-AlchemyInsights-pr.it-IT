---
title: Uso della prevenzione della perdita dei dati nelle regole di trasporto
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915184"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="d4a86-102">Uso della prevenzione della perdita dei dati nelle regole di trasporto</span><span class="sxs-lookup"><span data-stu-id="d4a86-102">Using DLP in transport rules</span></span>

<span data-ttu-id="d4a86-103">Per integrare i criteri di prevenzione della perdita dei dati in un trasporto esistente, usare la condizione "**Se il messaggio contiene... informazioni riservate**" nell'impostazione della regola di trasporto.</span><span class="sxs-lookup"><span data-stu-id="d4a86-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="d4a86-104">\*\*Per ulteriori dettagli, vedere \*\*.</span><span class="sxs-lookup"><span data-stu-id="d4a86-104">**For more details, see:**</span></span>

- <span data-ttu-id="d4a86-105">Tipi di informazioni riservate per la prevenzione della perdita dei dati integrate nelle regole di trasporto: [Integrare le regole sulle informazioni riservate](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="d4a86-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="d4a86-106">È anche possibile testare la regola con o senza test dei criteri usando la modalità di test sulla regola.</span><span class="sxs-lookup"><span data-stu-id="d4a86-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="d4a86-107">Attendere 30 minuti dopo la creazione della regola prima di eseguirne il test.</span><span class="sxs-lookup"><span data-stu-id="d4a86-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="d4a86-108">Vedere [Testare le regole del flusso di posta/di trasporto](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="d4a86-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="d4a86-109">**Nota**: se si sta cercando di implementare nuovi criteri di prevenzione della perdita dei dati con le regole di trasporto nell'interfaccia di amministrazione di Exchange, usare i [criteri di prevenzione della perdita dei dati nel Centro sicurezza e conformità](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="d4a86-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
