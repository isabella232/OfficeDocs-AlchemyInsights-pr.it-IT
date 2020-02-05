---
title: Creare un sito in SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770427"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="c9ea5-102">Creare siti di SharePoint mediante modelli</span><span class="sxs-lookup"><span data-stu-id="c9ea5-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="c9ea5-103">La possibilità di salvare un sito come modello non è supportata con i siti di comunicazione o di Team moderni.</span><span class="sxs-lookup"><span data-stu-id="c9ea5-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="c9ea5-104">Per ulteriori informazioni sull'utilizzo dei modelli [, vedere Salvataggio, download e caricamento di un sito di SharePoint come modello](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="c9ea5-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="c9ea5-105">Di seguito sono riportate alcune soluzioni o problemi comuni relativi al salvataggio di un sito o di un elenco come modello in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c9ea5-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="c9ea5-106">**Il pulsante Salva modello di sito/elenco non è disponibile o mancante**</span><span class="sxs-lookup"><span data-stu-id="c9ea5-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="c9ea5-107">Gli amministratori dovranno consentire lo script personalizzato per abilitare le caratteristiche del modello.</span><span class="sxs-lookup"><span data-stu-id="c9ea5-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="c9ea5-108">Per la procedura dettagliata, esempi e considerazioni vedere</span><span class="sxs-lookup"><span data-stu-id="c9ea5-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="c9ea5-109">Consentire o impedire lo script personalizzato</span><span class="sxs-lookup"><span data-stu-id="c9ea5-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="c9ea5-110">Il comando Salva sito come modello non è supportato e può causare problemi nei siti che utilizzano l'infrastruttura di pubblicazione di SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="c9ea5-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="c9ea5-111">**Il modello di sito non può essere creato o non funziona correttamente**</span><span class="sxs-lookup"><span data-stu-id="c9ea5-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="c9ea5-112">Il modello può mancare una [funzionalità](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) e non viene attivato.</span><span class="sxs-lookup"><span data-stu-id="c9ea5-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="c9ea5-113">Se la funzionalità non è disponibile per l'attivazione nella raccolta siti corrente, non è possibile utilizzare il modello di sito per creare un sito.</span><span class="sxs-lookup"><span data-stu-id="c9ea5-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="c9ea5-114">Controllare se gli elenchi o le raccolte superano la [soglia di limite per la visualizzazione elenco](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) di 5000 elementi, in quanto è possibile bloccare la creazione di un modello di sito.</span><span class="sxs-lookup"><span data-stu-id="c9ea5-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="c9ea5-115">Il sito può utilizzare troppe risorse e quindi il modello di sito supera il limite di 50 MB.</span><span class="sxs-lookup"><span data-stu-id="c9ea5-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="c9ea5-116">Sono presenti problemi durante la visualizzazione di dati da un elenco che utilizza una colonna di ricerca.</span><span class="sxs-lookup"><span data-stu-id="c9ea5-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="c9ea5-117">Per ulteriori informazioni, vedere [elenco generato da modelli non Visualizza i dati dell'elenco di ricerca corretto in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="c9ea5-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="c9ea5-118">Per informazioni più dettagliate su problemi e soluzioni comuni, vedere [creare e utilizzare modelli di sito](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="c9ea5-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



