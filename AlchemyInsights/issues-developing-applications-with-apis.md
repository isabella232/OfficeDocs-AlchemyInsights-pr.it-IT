---
title: Problemi di sviluppo di applicazioni con API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951901"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="9956e-102">Problemi di sviluppo di applicazioni con API</span><span class="sxs-lookup"><span data-stu-id="9956e-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="9956e-103">Per iniziare a utilizzare l'API di Azure Active Directory Graph, vedere la [Guida introduttiva](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) all'API di Azure AD Graph o visualizzare la [documentazione di riferimento relativa all'API di Azure AD Graph interattiva](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="9956e-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="9956e-104">**Fine del supporto di Azure Active Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="9956e-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="9956e-105">A **partire dal 30 giugno 2020**, non verranno più aggiunte nuove funzionalità a adal e Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="9956e-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="9956e-106">Si continuerà a fornire supporto tecnico e aggiornamenti per la sicurezza, ma non verranno più forniti aggiornamenti delle funzionalità.</span><span class="sxs-lookup"><span data-stu-id="9956e-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="9956e-107">**A partire dal 30 giugno 2022**, si finirà il supporto per adal e Azure AD Graph e non verranno più forniti supporto tecnico o aggiornamenti per la sicurezza.</span><span class="sxs-lookup"><span data-stu-id="9956e-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="9956e-108">Le app che utilizzano ADAL nelle versioni del sistema operativo esistenti continueranno a funzionare dopo questo periodo, ma non riceveranno alcun supporto tecnico o aggiornamenti per la sicurezza.</span><span class="sxs-lookup"><span data-stu-id="9956e-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="9956e-109">Le app che utilizzano Azure AD Graph dopo questo intervallo di tempo potrebbero non ricevere più risposte dall'endpoint di Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="9956e-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="9956e-110">**Migrazione ADAL**</span><span class="sxs-lookup"><span data-stu-id="9956e-110">**ADAL Migration**</span></span>

<span data-ttu-id="9956e-111">È consigliabile eseguire l'aggiornamento a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), in cui sono disponibili le funzionalità e gli aggiornamenti della sicurezza più recenti.</span><span class="sxs-lookup"><span data-stu-id="9956e-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="9956e-112">Se si utilizzano le app Microsoft, è necessario sapere che Microsoft sta eseguendo la migrazione delle applicazioni a MSAL in base alla scadenza del supporto tecnico, garantendo che possano usufruire dei miglioramenti della sicurezza e delle funzionalità di MSAL in corso.</span><span class="sxs-lookup"><span data-stu-id="9956e-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="9956e-113">[Leggere le domande frequenti su adal](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="9956e-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="9956e-114">Informazioni su [come eseguire la migrazione delle app per ogni singola piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="9956e-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="9956e-115">Se si ha bisogno di assistenza per capire quali app utilizzano ADAL, si consiglia di esaminare tutti i codici sorgente delle app e, se applicabile, di raggiungere tutti gli ISV o i provider di applicazioni.</span><span class="sxs-lookup"><span data-stu-id="9956e-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="9956e-116">Il supporto tecnico Microsoft può anche fornire un elenco di tutte le app di ADAL non Microsoft nel tenant.</span><span class="sxs-lookup"><span data-stu-id="9956e-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="9956e-117">**Migrazione del grafico AAD**</span><span class="sxs-lookup"><span data-stu-id="9956e-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="9956e-118">Per le applicazioni che utilizzano Azure AD Graph, seguire le istruzioni riportate di seguito per eseguire la migrazione delle [app di Azure AD Graph a Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="9956e-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="9956e-119">[L'elenco di controllo per la migrazione fornisce un punto introduttivo](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="9956e-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="9956e-120">Il portale di registrazione delle app di Azure indica le applicazioni che utilizzano il grafico AAD.</span><span class="sxs-lookup"><span data-stu-id="9956e-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="9956e-121">È consigliabile esaminare tutti i codici sorgente delle app e, se applicabile, rivolgersi a qualsiasi ISV o provider di applicazioni.</span><span class="sxs-lookup"><span data-stu-id="9956e-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="9956e-122">Il supporto tecnico Microsoft può anche fornire un elenco di tutti gli utilizzi del grafico AAD nel tenant.</span><span class="sxs-lookup"><span data-stu-id="9956e-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="9956e-123">Affinché l'app acceda ai dati in Microsoft Graph, l'utente o l'amministratore deve concedergli le autorizzazioni corrette tramite un processo di consenso.</span><span class="sxs-lookup"><span data-stu-id="9956e-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="9956e-124">La Guida di riferimento per le [autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) elenca le autorizzazioni associate a ciascun set principale di API di Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9956e-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="9956e-125">Vengono inoltre fornite indicazioni su come utilizzare le autorizzazioni.</span><span class="sxs-lookup"><span data-stu-id="9956e-125">It also provides guidance about how to use the permissions.</span></span>
