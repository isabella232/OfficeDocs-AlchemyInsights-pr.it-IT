---
title: 'Errore: le regole del computer non corrispondono'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664250"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="289d8-102">Errore: le regole del computer non corrispondono</span><span class="sxs-lookup"><span data-stu-id="289d8-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="289d8-103">Per visualizzare lo stato aggiornato di questo problema noto, vedere [le regole in questo computer non corrispondono alle regole di Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="289d8-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="289d8-104">Il team di Outlook ha implementato una correzione nella build 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="289d8-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="289d8-105">La correzione è già in Insider Fast e passerà a Monthly Channel alla fine di giugno 2020.</span><span class="sxs-lookup"><span data-stu-id="289d8-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="289d8-106">Dopo aver creato la build fissa, è possibile che venga visualizzato il messaggio "quali regole si desidera mantenere" un'ultima volta.</span><span class="sxs-lookup"><span data-stu-id="289d8-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="289d8-107">Quando viene richiesto, scegliere Server e quindi tornare indietro in Outlook e riattivare le regole disabilitate.</span><span class="sxs-lookup"><span data-stu-id="289d8-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="289d8-108">Fino a quando non è disponibile la correzione, utilizzare la soluzione seguente:</span><span class="sxs-lookup"><span data-stu-id="289d8-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="289d8-109">**Soluzione**: nei rapporti recenti, si è verificato il problema per gli utenti che hanno creato solo le regole client in Outlook desktop.</span><span class="sxs-lookup"><span data-stu-id="289d8-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="289d8-110">Se si continua a eseguire il problema, prendere in considerazione l'eliminazione delle regole e quindi creare e modificare le regole solo in OWA (Outlook Web App) fino a quando il problema non viene risolto.</span><span class="sxs-lookup"><span data-stu-id="289d8-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="289d8-111">Se non è possibile eliminare le regole manualmente, è possibile eseguire un comando di Outlook all'avvio di Outlook eseguendo Outlook. exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="289d8-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="289d8-112">Questo eliminerà sia le regole client che quelle del server.</span><span class="sxs-lookup"><span data-stu-id="289d8-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="289d8-113">Eliminerà tutte le regole per tutti gli account nel profilo di Outlook.</span><span class="sxs-lookup"><span data-stu-id="289d8-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="289d8-114">Questo comando è ulteriormente documentato nell'articolo delle opzioni della riga di comando.</span><span class="sxs-lookup"><span data-stu-id="289d8-114">This command is further documented in the Command-line switches article.</span></span>

