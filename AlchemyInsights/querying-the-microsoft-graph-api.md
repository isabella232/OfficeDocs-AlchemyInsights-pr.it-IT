---
title: Esecuzione di query nell'API di Microsoft Graph
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950715"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="0e4ce-102">Esecuzione di query nell'API di Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="0e4ce-103">Questo argomento potrebbe essere valido anche per gli sviluppatori che utilizzano ancora Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="0e4ce-104">Tuttavia, **è consigliabile utilizzare** Microsoft Graph per tutti gli scenari di gestione delle directory, delle identità e degli accessi.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="0e4ce-105">**Problemi di autenticazione o autorizzazione**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="0e4ce-106">Se l'app **non è in grado di acquisire token** per chiamare Microsoft Graph, scegli **un problema con la categoria ottenere un token di accesso (autenticazione)** di Microsoft Graph per ottenere assistenza e supporto più specifici su questo argomento.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="0e4ce-107">Se l'app **riceve gli errori di autorizzazione 401 o 403** quando si chiama Microsoft Graph, scegliere la categoria **ottenere un errore di accesso negato (autorizzazione)** Microsoft Graph API per ottenere assistenza e supporto più specifiche su questo argomento.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="0e4ce-108">**Si desidera utilizzare Microsoft Graph, ma non si è certi da dove iniziare**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="0e4ce-109">Per ulteriori informazioni su Microsoft Graph, vedere:</span><span class="sxs-lookup"><span data-stu-id="0e4ce-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="0e4ce-110">Panoramica di Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="0e4ce-111">Panoramica della gestione delle identità e degli accessi in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="0e4ce-112">Guida introduttiva alla creazione di app di Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="0e4ce-113">**Microsoft Graph Explorer** -testare le API di Microsoft Graph nel tenant o un tenant demo</span><span class="sxs-lookup"><span data-stu-id="0e4ce-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="0e4ce-114">**Si desidera utilizzare Microsoft Graph, ma supporta le API della directory v 1.0 di cui ho bisogno?**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="0e4ce-115">Microsoft Graph è l'API consigliata per la gestione delle directory, dell'identità e degli accessi.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="0e4ce-116">Tuttavia, vi sono ancora alcuni spazi vuoti tra ciò che è possibile fare in Azure AD Graph e Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="0e4ce-117">Esaminare gli articoli seguenti, in cui vengono evidenziate le differenze più aggiornate per facilitare la scelta:</span><span class="sxs-lookup"><span data-stu-id="0e4ce-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="0e4ce-118">Differenze tra i tipi di risorse tra Azure AD Graph e Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="0e4ce-119">Differenze tra le proprietà tra Azure AD Graph e Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="0e4ce-120">Differenze di metodo tra Azure AD e Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="0e4ce-121">**Quando si esegue una query sull'oggetto *utente* , molte delle relative proprietà sono mancanti**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="0e4ce-122">`GET https://graph.microsoft.com/v1.0/users` restituisce solo 11 proprietà, in quanto Microsoft Graph seleziona automaticamente un insieme predefinito di proprietà *utente* da restituire.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="0e4ce-123">Se sono necessarie altre proprietà *degli utenti* , utilizzare $Select per scegliere le proprietà necessarie per l'applicazione.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="0e4ce-124">Provare in **Microsoft Graph Explorer** per primo.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="0e4ce-125">**Alcuni valori delle proprietà utente sono *null* anche se sono stati impostati**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="0e4ce-126">La spiegazione più probabile è che all'applicazione sia stata concessa l'autorizzazione *User. ReadBasic. All* .</span><span class="sxs-lookup"><span data-stu-id="0e4ce-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="0e4ce-127">In questo modo l'applicazione può leggere un insieme limitato di proprietà dell'utente, restituendo tutte le altre proprietà come null anche se sono stati precedentemente impostati.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="0e4ce-128">Provare a concedere invece l'autorizzazione *User. Read. All* dell'applicazione.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="0e4ce-129">Per ulteriori informazioni, vedere [autorizzazioni utente di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="0e4ce-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="0e4ce-130">**Si verificano problemi con i parametri di query OData per filtrare i dati nelle richieste personali**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="0e4ce-131">Mentre Microsoft Graph supporta una vasta gamma di parametri di query OData, molti di questi parametri non sono completamente supportati dai servizi directory (risorse che ereditano da *directoryObject*) in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="0e4ce-132">Le stesse limitazioni presenti in Azure AD Graph persistono per la maggior parte in Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="0e4ce-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="0e4ce-133">**Non supportato**: $count, $search e $Filter su valori *null* o *non null*</span><span class="sxs-lookup"><span data-stu-id="0e4ce-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="0e4ce-134">**Non supportato**: $Filter su determinate proprietà (vedere Resource topics on quali proprietà sono filtrabili)</span><span class="sxs-lookup"><span data-stu-id="0e4ce-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="0e4ce-135">**Non supportato**: paging, filtro e ordinamento allo stesso tempo</span><span class="sxs-lookup"><span data-stu-id="0e4ce-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="0e4ce-136">**Non supportato**: filtro su una relazione.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="0e4ce-137">Ad esempio, trovare tutti i membri del gruppo di ingegneri che si trovano nel Regno Unito.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="0e4ce-138">**Supporto parziale**: $OrderBy su *utente* (solo DisplayName e userPrincipalName) e *gruppo*</span><span class="sxs-lookup"><span data-stu-id="0e4ce-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="0e4ce-139">**Supporto parziale**: $Filter (supporta solo il supporto di *EQ*, *StartsWith* *o* *, e e limitate*), $Expand (l'espansione delle relazioni di un singolo oggetto restituisce tutte le relazioni, ma l'espansione di una raccolta di relazioni degli oggetti è *limitata)*</span><span class="sxs-lookup"><span data-stu-id="0e4ce-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="0e4ce-140">Per ulteriori informazioni, vedere [Customize Responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0e4ce-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="0e4ce-141">**L'API che chiamo non funziona-dove è possibile eseguire altre operazioni di testing?**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="0e4ce-142">**Microsoft Graph Explorer** -testare le API di Microsoft Graph nel tenant o un tenant demo e consultare anche le **query di esempio** in Esplora risorse di Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="0e4ce-143">**Quando si esegue una query per i dati, sembra che venga restituito un set di dati incompleto**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="0e4ce-144">Se si esegue una query su un insieme (come *gli utenti*), Microsoft Graph utilizza limiti di pagina sul fianco del server in modo che i risultati vengano sempre restituiti con una dimensione di pagina predefinita.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="0e4ce-145">L'app dovrebbe sempre aspettarsi di passare alla pagina tramite gli insiemi restituiti dal servizio.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="0e4ce-146">Per altre informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="0e4ce-146">For more information, see:</span></span>

- [<span data-ttu-id="0e4ce-147">Procedure consigliate di Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="0e4ce-148">Paging dei dati di Microsoft Graph nell'app</span><span class="sxs-lookup"><span data-stu-id="0e4ce-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="0e4ce-149">**L'app è troppo lenta e viene anche strozzata. Quali miglioramenti è possibile apportare?**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="0e4ce-150">A seconda dello scenario, sono disponibili diverse opzioni per rendere l'applicazione più performante e, in alcuni casi, meno incline a essere strozzata dal servizio (quando si effettuano troppe chiamate).</span><span class="sxs-lookup"><span data-stu-id="0e4ce-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="0e4ce-151">Per altre informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="0e4ce-151">To learn more, see:</span></span>

- [<span data-ttu-id="0e4ce-152">Procedure consigliate di Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="0e4ce-153">Richieste di batch</span><span class="sxs-lookup"><span data-stu-id="0e4ce-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="0e4ce-154">Registrare le modifiche tramite la query Delta</span><span class="sxs-lookup"><span data-stu-id="0e4ce-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="0e4ce-155">Ricevere una notifica delle modifiche tramite webhook</span><span class="sxs-lookup"><span data-stu-id="0e4ce-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="0e4ce-156">Linee guida per la limitazione</span><span class="sxs-lookup"><span data-stu-id="0e4ce-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="0e4ce-157">**Dove è possibile trovare ulteriori informazioni sugli errori e sui problemi noti?**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="0e4ce-158">Informazioni sulla risposta di errore di Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="0e4ce-159">Problemi noti relativi a Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0e4ce-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="0e4ce-160">**Dove è possibile controllare lo stato della disponibilità e della connettività del servizio?**</span><span class="sxs-lookup"><span data-stu-id="0e4ce-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="0e4ce-161">La disponibilità del servizio e la connettività dei servizi sottostanti a cui è possibile accedere tramite Microsoft Graph possono influire sulla disponibilità complessiva e sulle prestazioni di Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0e4ce-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="0e4ce-162">Per l'integrità dei servizi di Azure Active Directory, controllare lo stato di **Security + Identity** Services elencato nella [pagina di stato di Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="0e4ce-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="0e4ce-163">Per i servizi di Office che contribuiscono a Microsoft Graph, controllare lo stato dei servizi elencati nel [dashboard di integrità del servizio di Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="0e4ce-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
