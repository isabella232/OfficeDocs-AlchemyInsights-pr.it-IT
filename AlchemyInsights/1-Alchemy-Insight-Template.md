---
title: 'uguale al nome del file è la migliore [RULE #-Description]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634508"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="373a5-102">Obbligatorio intestazione di alchimia H1, H2's non funziona.</span><span class="sxs-lookup"><span data-stu-id="373a5-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="373a5-103">Procedure consigliate e linee guida per la creazione di alchimia:</span><span class="sxs-lookup"><span data-stu-id="373a5-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="373a5-104">**Non annidare Insights alchimia nelle cartelle**-questo si romperà la struttura URL.</span><span class="sxs-lookup"><span data-stu-id="373a5-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="373a5-105">Stiamo cercando di risolvere la cosa.</span><span class="sxs-lookup"><span data-stu-id="373a5-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="373a5-106">I file nella cartella **AlchemyInsights** devono disporre dell'ID regola e del nome della regola dal [portale del partner](https://alchemyportal.azurewebsites.net) di alchimia nel nome del file.</span><span class="sxs-lookup"><span data-stu-id="373a5-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="373a5-107">ex.</span><span class="sxs-lookup"><span data-stu-id="373a5-107">ex.</span></span> <span data-ttu-id="373a5-108">***976-How-to-Enable-controversia legale-conservazione***</span><span class="sxs-lookup"><span data-stu-id="373a5-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="373a5-109">Utilizzare i metadati nella parte superiore del file come modello.</span><span class="sxs-lookup"><span data-stu-id="373a5-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="373a5-110">Non è necessario nient'altro.</span><span class="sxs-lookup"><span data-stu-id="373a5-110">Nothing else is required.</span></span>
1. <span data-ttu-id="373a5-111">Nel [portale del partner Alchemy](https://alchemyportal.azurewebsites.net), passare alla sezione **Customer Insight title:** e utilizzarlo come punto di partenza per il titolo H1 per Insight.</span><span class="sxs-lookup"><span data-stu-id="373a5-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="373a5-112">L'alchimia Insights deve avere solo un singolo H1 nella parte superiore o si romperà in produzione.</span><span class="sxs-lookup"><span data-stu-id="373a5-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="373a5-113">Non è possibile eseguire il rendering di H2s in modo da utilizzare convenzioni **audaci** o altre per indicare sezioni separate.</span><span class="sxs-lookup"><span data-stu-id="373a5-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="373a5-114">Successivamente, inserire il testo del corpo usando il materiale bozza nella sezione Customer Insights della pagina della regola di alchimia</span><span class="sxs-lookup"><span data-stu-id="373a5-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="373a5-115">Gli elenchi puntati sono ottimali</span><span class="sxs-lookup"><span data-stu-id="373a5-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="373a5-116">Elenchi numerati troppo</span><span class="sxs-lookup"><span data-stu-id="373a5-116">Numbered lists too</span></span>
    1. <span data-ttu-id="373a5-117">**Grassetto** e *corsivo* sono a-OK</span><span class="sxs-lookup"><span data-stu-id="373a5-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="373a5-118">I collegamenti devono essere sempre **"collegamenti al Web"/External** o **collegamenti profondi a elementi dell'interfaccia utente**, non collegamenti interni.</span><span class="sxs-lookup"><span data-stu-id="373a5-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="373a5-119">E questo è già un po' troppo lungo.</span><span class="sxs-lookup"><span data-stu-id="373a5-119">And this is really already a bit too long.</span></span> <span data-ttu-id="373a5-120">La procedura consigliata è di circa 400 caratteri---------------------------------</span><span class="sxs-lookup"><span data-stu-id="373a5-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="373a5-121">Una volta che il contenuto è pronto, tirarlo sul ramo Live.</span><span class="sxs-lookup"><span data-stu-id="373a5-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="373a5-122">Passare quindi al portale del [partner](https://alchemyportal.azurewebsites.net) di alchimia e immettere il nome del file nel campo URL.</span><span class="sxs-lookup"><span data-stu-id="373a5-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="373a5-123">Assicurarsi che Insight revisionato e pubblicato dica "Sì" e quindi fare clic su Aggiorna regola.</span><span class="sxs-lookup"><span data-stu-id="373a5-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="373a5-124">**(Questo aspetto sarà più bello nella nuova versione del portale-rilasciando al più presto).** 
 ![campo URL](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="373a5-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

