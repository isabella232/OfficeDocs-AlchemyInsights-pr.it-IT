---
title: Eseguire l'individuazione dei siti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529313"
---
# <a name="do-site-discovery"></a><span data-ttu-id="c3124-102">Eseguire l'individuazione dei siti</span><span class="sxs-lookup"><span data-stu-id="c3124-102">Do site discovery</span></span>

<span data-ttu-id="c3124-103">Se l'organizzazione usa ancora versioni legacy di applicazioni e piani Web e si prevede di utilizzare la modalità Internet Explorer, come la maggior parte dei clienti, occorre eseguire un'ulteriore individuazione dei siti.</span><span class="sxs-lookup"><span data-stu-id="c3124-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="c3124-104">**È già stata distribuita una versione precedente di Microsoft Edge**</span><span class="sxs-lookup"><span data-stu-id="c3124-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="c3124-105">Se è già stato configurato l'elenco dei siti modalità Enterprise in modo che funzioni per la versione legacy di Microsoft Edge, l'individuazione dei siti è quasi completata.</span><span class="sxs-lookup"><span data-stu-id="c3124-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="c3124-106">L'unica cosa che occorre fare è aggiungere siti neutri.</span><span class="sxs-lookup"><span data-stu-id="c3124-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="c3124-107">In genere i siti neutri sono siti che forniscono Single Sign-On (SSO).</span><span class="sxs-lookup"><span data-stu-id="c3124-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="c3124-108">Se si passa a un sito neutro da Microsoft Edge, è possibile usare Microsoft Edge per eseguire l'autenticazione.</span><span class="sxs-lookup"><span data-stu-id="c3124-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="c3124-109">Se si passa a un sito neutro in modalità Internet Explorer, è possibile usare la modalità Internet Explorer per eseguire l'autenticazione.</span><span class="sxs-lookup"><span data-stu-id="c3124-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="c3124-110">Identificare tutti i siti SSO o altri siti neutri utilizzati e aggiungerli all'elenco dei siti modalità Enterprise.</span><span class="sxs-lookup"><span data-stu-id="c3124-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="c3124-111">**Internet Explorer è il browser predefinito**.</span><span class="sxs-lookup"><span data-stu-id="c3124-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="c3124-112">Se si usa solo Internet Explorer, è probabile che non si sappia quali siti sono stati aggiornati agli standard Web moderni e richiedono ancora Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="c3124-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="c3124-113">È possibile trovare e aggiungere questi siti all'elenco dei siti modalità Enterprise in modo da poter usare la modalità Internet Explorer solo per tali siti.</span><span class="sxs-lookup"><span data-stu-id="c3124-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="c3124-114">[Individuazione di siti modalità Enterprise](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery): individua i siti che potrebbero richiedere la modalità Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="c3124-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="c3124-115">È possibile raccogliere dati nei computer che eseguono Windows Internet Explorer 8 tramite Internet Explorer 11 in Windows 10, Windows 8.1 o Windows 7.</span><span class="sxs-lookup"><span data-stu-id="c3124-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="c3124-116">**Analisi dei dati**.</span><span class="sxs-lookup"><span data-stu-id="c3124-116">**Analyze the data**</span></span>

<span data-ttu-id="c3124-117">Dopo aver raccolto i dati del sito, per analizzare i dati è consigliabile eseguire il processo in 4 passaggi riportato di seguito:</span><span class="sxs-lookup"><span data-stu-id="c3124-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="c3124-118">Ordinare i dati in base al dominio, quindi in base all'URL.</span><span class="sxs-lookup"><span data-stu-id="c3124-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="c3124-119">Definire i limiti di un'app da configurare per la modalità Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="c3124-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="c3124-120">È possibile includere tutti i siti e i controlli Web che definiscono l'app, ma non è possibile includere altri siti e controlli.</span><span class="sxs-lookup"><span data-stu-id="c3124-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="c3124-121">Alcuni siti possono essere semplici, ad esempio *https://contoso.com/app1*, mentre altri possono richiedere la definizione di più siti e pagine.</span><span class="sxs-lookup"><span data-stu-id="c3124-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="c3124-122">Eseguire un test dell'app per verificare che non funzioni in modo nativo.</span><span class="sxs-lookup"><span data-stu-id="c3124-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="c3124-123">Molti siti offriranno contenuti moderni quando rilevano un browser moderno e solo contenuti legacy quando individuano Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="c3124-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="c3124-124">Aggiungere l'app all'elenco dei siti modalità Enterprise se non si riesce a eseguire il test.</span><span class="sxs-lookup"><span data-stu-id="c3124-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="c3124-125">Come procedura consigliata, raggruppare tutti i siti che comprendono un'app.</span><span class="sxs-lookup"><span data-stu-id="c3124-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="c3124-126">In questo modo, quando si aggiorna un'app, è più facile rimuovere l'intero sito dalla modalità Internet Explorer e iniziare a usare un browser moderno per l'app specifica.</span><span class="sxs-lookup"><span data-stu-id="c3124-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="c3124-127">Dopo aver completato l'individuazione dei siti e aver analizzato i dati, è possibile iniziare a considerare la strategia del canale.</span><span class="sxs-lookup"><span data-stu-id="c3124-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

