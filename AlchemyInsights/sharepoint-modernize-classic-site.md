---
title: Sito moderno come sito radice
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid:
- "9000153"
- "1692"
ms.openlocfilehash: 6f55f1c63551027cc5522d296cb3f3f342356d95
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36576688"
---
# <a name="modernize-your-classic-sharepoint-site"></a><span data-ttu-id="04482-102">Modernizzare il sito di SharePoint classico</span><span class="sxs-lookup"><span data-stu-id="04482-102">Modernize your classic SharePoint site</span></span>

<span data-ttu-id="04482-103">Per passare a un'interfaccia utente moderna, è necessario concentrarsi sui seguenti elementi:</span><span class="sxs-lookup"><span data-stu-id="04482-103">To make the switch to a modern user interface, you need to focus on the following:</span></span>

- <span data-ttu-id="04482-104">Transizione di **elenchi e raccolte** per l'utilizzo dell'interfaccia utente moderna (nota anche come l'elenco e l'esperienza di raccolta moderni).</span><span class="sxs-lookup"><span data-stu-id="04482-104">Transitioning your **lists and libraries** to use the modern user interface (also referred to as the modern list and library experience).</span></span>
- <span data-ttu-id="04482-105">Trasformando le **pagine del sito** da wiki classico e pagine Web part in moderne pagine sul lato client.</span><span class="sxs-lookup"><span data-stu-id="04482-105">Transforming your **site pages** from classic wiki and web part pages into modern client-side pages.</span></span>
- <span data-ttu-id="04482-106">Creazione di **siti moderni** (sito del team o sito di comunicazione).</span><span class="sxs-lookup"><span data-stu-id="04482-106">Creating **modern sites** (Team site or Communication Site).</span></span>

<span data-ttu-id="04482-107">Modernizzare l'esperienza per:</span><span class="sxs-lookup"><span data-stu-id="04482-107">Modernize your experience by:</span></span>
- <span data-ttu-id="04482-108">[Abilitazione di elenchi e raccolte per la visualizzazione nell'interfaccia utente moderna](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries) sostituendo le personalizzazioni, rimuovendo le colonne incompatibili dalle visualizzazioni utilizzate o (come ultima risorsa) spostando i dati in un tipo di elenco moderno compatibile con l'interfaccia utente.</span><span class="sxs-lookup"><span data-stu-id="04482-108">[Enabling lists and libraries to show in the modern user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries) by replacing customizations, removing incompatible columns from the used views, or (as a last resort) moving data into a modern user interface-compatible list type.</span></span>
- <span data-ttu-id="04482-109">[Connessione del sito a un gruppo di Office 365](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group), che conferisce al sito una Home page moderna e che consente di utilizzare il sito, ad esempio una cassetta postale o Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="04482-109">[Connecting your site to an Office 365 group](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group), which gives your site a modern home page and enables your site to use, for example, a mailbox or Microsoft Planner.</span></span> <span data-ttu-id="04482-110">In questo modo è possibile utilizzare una versione moderna di un elenco di calendario e attività.</span><span class="sxs-lookup"><span data-stu-id="04482-110">This enables you to use a modern version of a calendar and task list.</span></span>
- <span data-ttu-id="04482-111">La [creazione di pagine moderne](https://support.office.com/article/create-and-use-modern-pages-on-a-sharepoint-site-b3d46deb-27a6-4b1e-87b8-df851e503dec)è un ottimo modo per condividere idee con immagini, Excel, documenti di Word e PowerPoint, video e altro ancora.</span><span class="sxs-lookup"><span data-stu-id="04482-111">[Creating modern pages](https://support.office.com/article/create-and-use-modern-pages-on-a-sharepoint-site-b3d46deb-27a6-4b1e-87b8-df851e503dec), is a great way to share ideas using images, Excel, Word and PowerPoint documents, video, and more.</span></span>
- <span data-ttu-id="04482-112">[Creare pagine sul lato client moderne](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-site-pages) e configurarle come "simili" al wiki classico e alle pagine Web part principali.</span><span class="sxs-lookup"><span data-stu-id="04482-112">[Creating modern client-side pages](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-site-pages) and configuring these to be "similar" to your key classic wiki and web part pages.</span></span> <span data-ttu-id="04482-113">La trasformazione della pagina a livello di programmazione dovrebbe essere fatta per le pagine principali dei siti, in quanto la trasformazione di tutte le pagine richiede un utilizzo intensivo delle risorse e spesso non necessaria.</span><span class="sxs-lookup"><span data-stu-id="04482-113">Programmatic page transformation should be done for the key pages of your sites, as transforming all pages is resource-intensive and often not needed.</span></span> <span data-ttu-id="04482-114">Per facilitare questo tipo di valutazione, lo scanner di modernizzazione di SharePoint può fornire informazioni sull'utilizzo delle pagine wiki e Web part correnti.</span><span class="sxs-lookup"><span data-stu-id="04482-114">To assist in this triage, the SharePoint Modernization scanner can give you usage information about the current wiki and web part pages.</span></span>
- <span data-ttu-id="04482-115">[Creazione di siti moderni](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="04482-115">[Creating modern sites](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span> <span data-ttu-id="04482-116">È preferibile creare un sito del team o un sito di comunicazione?</span><span class="sxs-lookup"><span data-stu-id="04482-116">Should I create a team site or a communication site?</span></span>

<span data-ttu-id="04482-117">Ulteriori informazioni:</span><span class="sxs-lookup"><span data-stu-id="04482-117">Additional Info:</span></span> 
- <span data-ttu-id="04482-118">Per una panoramica dettagliata della modernizzazione dei siti di SharePoint classici all'esperienza moderna, vedere [modernizzare i siti di SharePoint classici](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites).</span><span class="sxs-lookup"><span data-stu-id="04482-118">For a step-by-step overview of modernizing your classic SharePoint Sites to the modern experience, see [Modernize your classic SharePoint Sites](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites).</span></span>
- <span data-ttu-id="04482-119">Consultare una guida all' [esperienza moderna](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience).</span><span class="sxs-lookup"><span data-stu-id="04482-119">See a guide to [Modern Experience](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience).</span></span>
- <span data-ttu-id="04482-120">Vedere [esperienze classiche e moderne di SharePoint](https://support.office.com/article/sharepoint-classic-and-modern-experiences-5725c103-505d-4a6e-9350-300d3ec7d73f).</span><span class="sxs-lookup"><span data-stu-id="04482-120">See [SharePoint Classic and Modern experiences](https://support.office.com/article/sharepoint-classic-and-modern-experiences-5725c103-505d-4a6e-9350-300d3ec7d73f).</span></span> 




