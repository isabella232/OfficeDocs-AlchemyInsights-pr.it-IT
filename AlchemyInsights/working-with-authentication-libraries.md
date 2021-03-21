---
title: Usare le raccolte di autenticazione
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897900"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="2ecbf-102">Usare le raccolte di autenticazione</span><span class="sxs-lookup"><span data-stu-id="2ecbf-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="2ecbf-103">Per risolvere il problema della raccolta MSAL, esegui i seguenti passaggi raccomandati:</span><span class="sxs-lookup"><span data-stu-id="2ecbf-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="2ecbf-104">**Usare la raccolta MSAL**: [Raccolta di autenticazione della piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - Questo articolo illustra il supporto della raccolta di autenticazione di Microsoft per diversi tipi di applicazioni.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="2ecbf-105">Include collegamenti al codice sorgente della raccolta; descrive dove ottenere il pacchetto per il progetto dell'app, se la raccolta supporta l'autenticazione dell'utente, come accedere online alle API protette o entrambi.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="2ecbf-106">**Risoluzione dei problemi di autenticazione**: la raccolta supporta numerosi flussi di autenticazione per l'uso in contesti applicativi differenti</span><span class="sxs-lookup"><span data-stu-id="2ecbf-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="2ecbf-107">A seconda di come viene creata l'applicazione client, la raccolta MSAL può usare uno o più flussi di autenticazione supportati dalla piattaforma Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="2ecbf-108">Questi flussi possono produrre diversi tipi di token e codici di autorizzazione, e richiede l'uso di token differenti per farli funzionare.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="2ecbf-109">**Token di accesso**: [token di accesso della piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Scopri come la tua API può convalidare e usare le attestazioni dei token di accesso.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="2ecbf-110">Tutta la documentazione di questo articolo, tranne quanto specificato, si applica solo ai token rilasciati per le API registrate.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="2ecbf-111">Non si applica ai token rilasciati per le API di proprietà di Microsoft, né può essere usata per convalidare il modo in cui la piattaforma Microsoft Identity emette i token per le API create dall'utente.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="2ecbf-112">**Fine del supporto per Azure Active Directory Authentication Library (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="2ecbf-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="2ecbf-113">**A partire dal 30 giugno 2020,** non aggiungeremo altre funzionalità ad ADAL e Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="2ecbf-114">Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="2ecbf-115">**A partire dal 30 giugno 2022,** Microsoft terminerà il supporto per ADAL e Graph di AAD e non fornirà più supporto tecnico o aggiornamenti della sicurezza.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="2ecbf-116">Le app che usano ADAL nelle versioni del sistema operativo esistenti continueranno a funzionare dopo tale data, ma non *riceveranno alcun supporto tecnico o aggiornamento di sicurezza*.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="2ecbf-117">Le app che usano Graph di Azure AD dopo tale data potrebbero non ricevere più risposte dall'endpoint Graph di Azure AD.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="2ecbf-118">**Migrazione ADAL**</span><span class="sxs-lookup"><span data-stu-id="2ecbf-118">**ADAL Migration**</span></span>

- <span data-ttu-id="2ecbf-119">Raccomandiamo di eseguire l'aggiornamento alla raccolta MSAL, che include le ultime funzionalità e gli aggiornamenti di sicurezza più recenti.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="2ecbf-120">Se usi Microsoft Apps, devi sapere che Microsoft sta completando la migrazione delle app su MSAL entro la data di scadenza del supporto, per assicurarsi che possano beneficiare dei miglioramenti continui della sicurezza e delle funzionalità di MSAL.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="2ecbf-121">[Leggi le domande frequenti su ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="2ecbf-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="2ecbf-122">[Informazioni su come eseguire la migrazione delle app in base alla piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="2ecbf-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="2ecbf-123">Se hai ancora dubbi dopo aver letto la guida per la piattaforma della tua app, puoi scrivere un post su [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) con il tag [azure-ad-adal-deprecation] o aprire un ticket nell'archivio GitHub della raccolta.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="2ecbf-124">Vedi la sezione [Lingue e framework](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) dell'articolo **Paroramica su MSAL** per i collegamenti agli archivi di ciascuna raccolta.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="2ecbf-125">**Se serve aiuto per capire quale app usa ADAL**, ti consigliamo di esaminare tutto il codice sorgente delle tue app.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="2ecbf-126">Se applicabile, contatta eventuali fornitori di software indipendenti (ISV) o provider di app.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="2ecbf-127">Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.</span><span class="sxs-lookup"><span data-stu-id="2ecbf-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







