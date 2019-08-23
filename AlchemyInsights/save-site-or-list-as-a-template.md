---
title: Salvare il sito o l'elenco come modello
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551635"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="df062-102">Salvare il sito o l'elenco come modello</span><span class="sxs-lookup"><span data-stu-id="df062-102">Save site or list as a template</span></span>

<span data-ttu-id="df062-103">I modelli di sito di SharePoint sono definizioni predefinite progettate attorno a una specifica esigenza aziendale.</span><span class="sxs-lookup"><span data-stu-id="df062-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="df062-104">Per ulteriori informazioni, vedere [utilizzo di modelli per creare diversi tipi di siti di SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="df062-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="df062-105">Di seguito sono riportate alcune soluzioni o problemi comuni relativi al salvataggio di un sito o di un elenco come modello in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="df062-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="df062-106">Il **pulsante Salva modello di sito/elenco non è disponibile o mancante**.</span><span class="sxs-lookup"><span data-stu-id="df062-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="df062-107">Gli amministratori dovranno consentire lo script personalizzato per abilitare le caratteristiche del modello.</span><span class="sxs-lookup"><span data-stu-id="df062-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="df062-108">Per la procedura dettagliata, esempi e considerazioni, vedere [Allow or impedisce script personalizzato](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="df062-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="df062-109">Il comando Salva sito come modello non è supportato e può causare problemi nei siti che utilizzano l'infrastruttura di pubblicazione di SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="df062-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="df062-110">**Il modello di sito non può essere creato o non funziona correttamente**</span><span class="sxs-lookup"><span data-stu-id="df062-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="df062-111">Il modello può mancare una [funzionalità](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e non viene attivato.</span><span class="sxs-lookup"><span data-stu-id="df062-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="df062-112">Se la funzionalità non è disponibile per l'attivazione nella raccolta siti corrente, non è possibile utilizzare il modello di sito per creare un sito.</span><span class="sxs-lookup"><span data-stu-id="df062-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="df062-113">Controllare se gli elenchi o le raccolte superano la [soglia di limite per la visualizzazione elenco](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) di 5000 elementi, in quanto è possibile bloccare la creazione di un modello di sito.</span><span class="sxs-lookup"><span data-stu-id="df062-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="df062-114">Il sito può utilizzare troppe risorse e quindi il modello di sito supera il limite di 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="df062-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="df062-115">Sono presenti problemi durante la visualizzazione di dati da un elenco che utilizza una colonna di ricerca.</span><span class="sxs-lookup"><span data-stu-id="df062-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="df062-116">Per ulteriori informazioni, vedere [elenco generato da modelli non Visualizza i dati dell'elenco di ricerca corretto in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="df062-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="df062-117">Per informazioni più dettagliate su problemi e soluzioni comuni, fare riferimento, [creare e utilizzare modelli di sito](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="df062-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

