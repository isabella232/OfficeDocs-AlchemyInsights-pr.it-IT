---
title: uguale al nome del file è la migliore
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/22/2019
ms.locfileid: "30762069"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="fd81f-102">Obbligatorio intestazione di alchimia H1, H2's non funziona.</span><span class="sxs-lookup"><span data-stu-id="fd81f-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="fd81f-103">Procedure consigliate e linee guida per la creazione di alchimia:</span><span class="sxs-lookup"><span data-stu-id="fd81f-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="fd81f-104">**Non annidare Insights alchimia nelle cartelle**-questo si romperà la struttura URL.</span><span class="sxs-lookup"><span data-stu-id="fd81f-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="fd81f-105">Stiamo cercando di risolvere la cosa.</span><span class="sxs-lookup"><span data-stu-id="fd81f-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="fd81f-106">I file presenti nella cartella **AlchemyInsights** devono avere nomi filecaratteri minuscoli con trattini per gli spazi ex.</span><span class="sxs-lookup"><span data-stu-id="fd81f-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="fd81f-107">***How-to-Enable-controversia legale-*** conservazione.</span><span class="sxs-lookup"><span data-stu-id="fd81f-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="fd81f-108">Includere l'ID della regola o l'ID del bucket dal [portale del partner di Alchemy](https://alchemyportal.azurewebsites.net) nel campo ms. Custom.</span><span class="sxs-lookup"><span data-stu-id="fd81f-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="fd81f-109">ex.</span><span class="sxs-lookup"><span data-stu-id="fd81f-109">ex.</span></span> <span data-ttu-id="fd81f-110">***ms. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="fd81f-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="fd81f-111">Utilizzare il resto dei metadati nella parte superiore del file come modello.</span><span class="sxs-lookup"><span data-stu-id="fd81f-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="fd81f-112">Nel [portale del partner Alchemy](https://alchemyportal.azurewebsites.net), passare alla sezione **Customer Insight title:** e utilizzarlo come punto di partenza per il titolo H1 per Insight.</span><span class="sxs-lookup"><span data-stu-id="fd81f-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="fd81f-113">L'alchimia Insights deve avere solo un singolo H1 nella parte superiore o si romperà in produzione.</span><span class="sxs-lookup"><span data-stu-id="fd81f-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="fd81f-114">Non è possibile eseguire il rendering di H2s in modo da utilizzare convenzioni **audaci** o altre per indicare sezioni separate.</span><span class="sxs-lookup"><span data-stu-id="fd81f-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="fd81f-115">Successivamente, inserire il testo del corpo usando il materiale bozza nella sezione Customer Insights della pagina della regola di alchimia</span><span class="sxs-lookup"><span data-stu-id="fd81f-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="fd81f-116">Gli elenchi puntati sono ottimali</span><span class="sxs-lookup"><span data-stu-id="fd81f-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="fd81f-117">Elenchi numerati troppo</span><span class="sxs-lookup"><span data-stu-id="fd81f-117">Numbered lists too</span></span>
    1. <span data-ttu-id="fd81f-118">**Grassetto** e *corsivo* sono a-OK</span><span class="sxs-lookup"><span data-stu-id="fd81f-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="fd81f-119">I collegamenti devono essere sempre **"collegamenti al Web"/External** o **collegamenti profondi a elementi dell'interfaccia utente**, non collegamenti interni.</span><span class="sxs-lookup"><span data-stu-id="fd81f-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="fd81f-120">Le immagini non sono supportate ufficialmente in questo momento, ma sono presenti nella roadmap.</span><span class="sxs-lookup"><span data-stu-id="fd81f-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="fd81f-121">E questo è già un po' troppo lungo.</span><span class="sxs-lookup"><span data-stu-id="fd81f-121">And this is really already a bit too long.</span></span> <span data-ttu-id="fd81f-122">La procedura consigliata è di circa 400 caratteri---------------------------------</span><span class="sxs-lookup"><span data-stu-id="fd81f-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="fd81f-123">Una volta che il contenuto è pronto, tirarlo sul ramo Live.</span><span class="sxs-lookup"><span data-stu-id="fd81f-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="fd81f-124">Passare quindi al portale del [partner](https://alchemyportal.azurewebsites.net) di alchimia e immettere il nome del file nel campo URL.</span><span class="sxs-lookup"><span data-stu-id="fd81f-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="fd81f-125">M</span><span class="sxs-lookup"><span data-stu-id="fd81f-125">M</span></span>