---
title: Problemi con le librerie di autenticazione
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037216"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="1efd0-102">Problemi con le librerie di autenticazione</span><span class="sxs-lookup"><span data-stu-id="1efd0-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="1efd0-103">[Le raccolte di autenticazione della piattaforma di](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) identità Microsoft elencano le librerie client e middleware supportate e compatibili da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1efd0-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="1efd0-104">Microsoft Authentication Library (MSAL) supporta diversi flussi [di autenticazione](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) da utilizzare in diversi scenari di applicazioni.</span><span class="sxs-lookup"><span data-stu-id="1efd0-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="1efd0-105">Per autenticare e acquisire token, inizializza una nuova applicazione client pubblica o riservata nel codice.</span><span class="sxs-lookup"><span data-stu-id="1efd0-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="1efd0-106">Puoi impostare diverse opzioni di configurazione quando inizializza l'app client in Microsoft Authentication Library (MSAL).</span><span class="sxs-lookup"><span data-stu-id="1efd0-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="1efd0-107">Per ulteriori informazioni, vedere [Opzioni di configurazione dell'applicazione.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)</span><span class="sxs-lookup"><span data-stu-id="1efd0-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="1efd0-108">**Fine del supporto per Azure Active Directory Authentication Library (ADAL) e Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="1efd0-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="1efd0-109">**A partire dal 30 giugno 2020,** non aggiungeremo più nuove funzionalità ad ADAL e Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="1efd0-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="1efd0-110">Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.</span><span class="sxs-lookup"><span data-stu-id="1efd0-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="1efd0-111">**A partire dal 30 giugno 2022,** microsoft terminerà il supporto per ADAL e Azure AD Graph e non fornirà più supporto tecnico o aggiornamenti della sicurezza.</span><span class="sxs-lookup"><span data-stu-id="1efd0-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="1efd0-112">Le app che usano ADAL nelle versioni esistenti del sistema operativo continueranno a funzionare dopo questo periodo, ma non riceveranno alcun supporto tecnico o aggiornamenti *della sicurezza.*</span><span class="sxs-lookup"><span data-stu-id="1efd0-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="1efd0-113">Le app che usano Azure AD Graph dopo questo periodo potrebbero non ricevere più risposte dall'endpoint di Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="1efd0-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="1efd0-114">**Migrazione ADAL**</span><span class="sxs-lookup"><span data-stu-id="1efd0-114">**ADAL Migration**</span></span>

<span data-ttu-id="1efd0-115">È consigliabile eseguire l'aggiornamento a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), che include le funzionalità e gli aggiornamenti della sicurezza più recenti.</span><span class="sxs-lookup"><span data-stu-id="1efd0-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="1efd0-116">Se si usano le app Microsoft, è importante sapere che Microsoft sta eseguendo la migrazione delle applicazioni a MSAL entro la scadenza del supporto, assicurandosi che trarranno vantaggio dai continui miglioramenti delle funzionalità e della sicurezza di MSAL.</span><span class="sxs-lookup"><span data-stu-id="1efd0-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="1efd0-117">Per altre informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="1efd0-117">For more information, see:</span></span>

1. [<span data-ttu-id="1efd0-118">Consultare le domande frequenti su ADAL</span><span class="sxs-lookup"><span data-stu-id="1efd0-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="1efd0-119">Informazioni su come eseguire la migrazione delle app in base alla piattaforma</span><span class="sxs-lookup"><span data-stu-id="1efd0-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="1efd0-120">Se ti serve aiuto per capire quale delle tue app usa ADAL, ti consigliamo di esaminare tutto il codice sorgente delle tue app e, se applicabile, contattare qualsiasi ISV o provider di app.</span><span class="sxs-lookup"><span data-stu-id="1efd0-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="1efd0-121">Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.</span><span class="sxs-lookup"><span data-stu-id="1efd0-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="1efd0-122">**Migrazione Graph di AAD**</span><span class="sxs-lookup"><span data-stu-id="1efd0-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="1efd0-123">Per le applicazioni che usano Azure AD Graph, seguire le indicazioni per eseguire la [migrazione delle app Di Azure AD Graph a Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="1efd0-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="1efd0-124">L'elenco di controllo per la migrazione fornisce un punto di partenza.</span><span class="sxs-lookup"><span data-stu-id="1efd0-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="1efd0-125">Il portale di registrazione delle app Azure illustra quali applicazioni usano Graph di AAD.</span><span class="sxs-lookup"><span data-stu-id="1efd0-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="1efd0-126">È consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti o provider di app.</span><span class="sxs-lookup"><span data-stu-id="1efd0-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="1efd0-127">Il supporto Tecnico Microsoft può anche fornire un elenco di tutti gli utilizzi di AAD Graph nel tenant.</span><span class="sxs-lookup"><span data-stu-id="1efd0-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="1efd0-128">Per consentire all'app di accedere ai dati in Microsoft Graph, l'utente o l'amministratore deve concedervi le autorizzazioni corrette tramite un processo di consenso.</span><span class="sxs-lookup"><span data-stu-id="1efd0-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="1efd0-129">Nella [guida di riferimento alle autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) sono elencate le autorizzazioni associate a ogni set principale di API di Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1efd0-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="1efd0-130">Vengono inoltre fornite indicazioni su come utilizzare le autorizzazioni.</span><span class="sxs-lookup"><span data-stu-id="1efd0-130">It also provides guidance about how to use the permissions.</span></span>
