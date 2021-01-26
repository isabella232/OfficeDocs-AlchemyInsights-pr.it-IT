---
title: Problemi relativi allo sviluppo di applicazioni
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950801"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="750d9-102">Problemi relativi allo sviluppo di applicazioni</span><span class="sxs-lookup"><span data-stu-id="750d9-102">Issues developing applications</span></span>

<span data-ttu-id="750d9-103">Per la risoluzione dei problemi più comuni durante la creazione di app Azure Active Directory (AD), vedere gli articoli seguenti:</span><span class="sxs-lookup"><span data-stu-id="750d9-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="750d9-104">Problemi di accesso alle applicazioni solo usando il browser Chrome</span><span class="sxs-lookup"><span data-stu-id="750d9-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="750d9-105">Come modificare le impostazioni predefinite di durata del token per l'applicazione</span><span class="sxs-lookup"><span data-stu-id="750d9-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="750d9-106">Come funziona il consenso dell'applicazione</span><span class="sxs-lookup"><span data-stu-id="750d9-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="750d9-107">Come concedere le autorizzazioni all'applicazione</span><span class="sxs-lookup"><span data-stu-id="750d9-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="750d9-108">Differenze tra le autorizzazioni delegate e le autorizzazioni dell'applicazione</span><span class="sxs-lookup"><span data-stu-id="750d9-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="750d9-109">\***Fine del supporto per Active Directory Authentication Library (ADAL) e l'API Graph di Azure AD (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="750d9-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="750d9-110">A partire dal 30 giugno 2020, non verranno più aggiunte nuove funzionalità ad Active Directory Authentication Library (ADAL) e all'API Graph di Azure AD (A AD Graph).</span><span class="sxs-lookup"><span data-stu-id="750d9-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="750d9-111">Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.</span><span class="sxs-lookup"><span data-stu-id="750d9-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="750d9-112">A partire dal 30 giugno 2022, Microsoft terminerà il supporto per ADAL e Graph di AAD e non fornirà più supporto tecnico o aggiornamenti della sicurezza.</span><span class="sxs-lookup"><span data-stu-id="750d9-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="750d9-113">In considerazione di quanto illustrato in precedenza, le implicazioni sono le seguenti:</span><span class="sxs-lookup"><span data-stu-id="750d9-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="750d9-114">Le app che usano ADAL nelle versioni del sistema operativo esistenti continueranno a funzionare dopo tale data, ma non riceveranno alcun supporto tecnico o aggiornamento della sicurezza.</span><span class="sxs-lookup"><span data-stu-id="750d9-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="750d9-115">Le app che usano Graph di AAD dopo tale data potrebbero non ricevere più risposte dall'endpoint Graph di AAD</span><span class="sxs-lookup"><span data-stu-id="750d9-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="750d9-116">_ *Migrazione ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="750d9-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="750d9-117">Se si usano app Microsoft, è consigliabile eseguire l'aggiornamento a Microsoft Authentication Library (MSAL), che include le funzionalità e gli aggiornamenti della sicurezza più recenti.</span><span class="sxs-lookup"><span data-stu-id="750d9-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="750d9-118">Questo suggerimento è valido nel caso in cui Microsoft avvii il processo di migrazione delle app a MSAL prima della scadenza del supporto.</span><span class="sxs-lookup"><span data-stu-id="750d9-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="750d9-119">Tramite la migrazione a MSAL da parte di Microsoft, le app beneficeranno dei vantaggi derivanti dai continui miglioramenti della sicurezza e delle funzionalità di MSAL.</span><span class="sxs-lookup"><span data-stu-id="750d9-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="750d9-120">Consultare le domande frequenti su ADAL</span><span class="sxs-lookup"><span data-stu-id="750d9-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="750d9-121">Informazioni su come eseguire la migrazione delle app in base alla piattaforma</span><span class="sxs-lookup"><span data-stu-id="750d9-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="750d9-122">Se serve assistenza per capire quale app usa ADAL, è consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti (ISV) o provider di app.</span><span class="sxs-lookup"><span data-stu-id="750d9-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="750d9-123">Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.</span><span class="sxs-lookup"><span data-stu-id="750d9-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="750d9-124">**Migrazione Graph di AAD**</span><span class="sxs-lookup"><span data-stu-id="750d9-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="750d9-125">Per le applicazioni che usano Graph di AAD, seguire le indicazioni per la migrazione delle app Graph di AAD a Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="750d9-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="750d9-126">[L'elenco di controllo per la migrazione fornisce un punto di partenza](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="750d9-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="750d9-127">Il portale di registrazione delle app Azure illustra quali applicazioni usano Graph di AAD.</span><span class="sxs-lookup"><span data-stu-id="750d9-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="750d9-128">È consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti o provider di app.</span><span class="sxs-lookup"><span data-stu-id="750d9-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="750d9-129">Il supporto Microsoft può fornire informazioni sull'utilizzo di Graph di AAD nel tenant.</span><span class="sxs-lookup"><span data-stu-id="750d9-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







