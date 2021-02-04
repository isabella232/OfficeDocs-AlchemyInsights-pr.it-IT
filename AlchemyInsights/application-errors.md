---
title: Errori dell'applicazione
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
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976916"
---
# <a name="application-errors"></a><span data-ttu-id="b781e-102">Errori dell'applicazione</span><span class="sxs-lookup"><span data-stu-id="b781e-102">Application errors</span></span>

<span data-ttu-id="b781e-103">Per informazioni sui codici di **errore di AADSTS** restituiti dal servizio token di sicurezza (STS) di Azure Active Directory (Azure ad)?</span><span class="sxs-lookup"><span data-stu-id="b781e-103">Looking for info about the **AADSTS error codes** that are returned from the Azure Active Directory (Azure AD) security token service (STS)?</span></span> <span data-ttu-id="b781e-104">Leggere i [codici di errore per l'autenticazione e l'autorizzazione di Azure ad](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) per individuare le descrizioni degli errori di AADSTS, le correzioni e alcune soluzioni alternative consigliate.</span><span class="sxs-lookup"><span data-stu-id="b781e-104">Read [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>

<span data-ttu-id="b781e-105">Gli errori di autorizzazione possono essere causati da diversi problemi, la maggior parte dei quali genera un errore 401 o 403.</span><span class="sxs-lookup"><span data-stu-id="b781e-105">Authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="b781e-106">Ad esempio, i seguenti elementi possono portare a errori di autorizzazione:</span><span class="sxs-lookup"><span data-stu-id="b781e-106">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="b781e-107">[Flussi di acquisizione di token di accesso](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) non corretti</span><span class="sxs-lookup"><span data-stu-id="b781e-107">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)</span></span> 
- <span data-ttu-id="b781e-108">[Ambiti di autorizzazione](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) mal configurati</span><span class="sxs-lookup"><span data-stu-id="b781e-108">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span> 
- <span data-ttu-id="b781e-109">Mancanza di [consenso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="b781e-109">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="b781e-110">Per risolvere gli errori di autorizzazione comuni, provare a eseguire i passaggi riportati di seguito che corrispondono più fedelmente all'errore che si sta ricevendo.</span><span class="sxs-lookup"><span data-stu-id="b781e-110">To resolve common authorization errors, try the steps provided below that most closely matches the error you are receiving.</span></span> <span data-ttu-id="b781e-111">È possibile applicare più di uno.</span><span class="sxs-lookup"><span data-stu-id="b781e-111">More than one may apply.</span></span>

<span data-ttu-id="b781e-112">**401 errore non autorizzato: il token è valido?**</span><span class="sxs-lookup"><span data-stu-id="b781e-112">**401 Unauthorized error: Is your token valid?**</span></span>

<span data-ttu-id="b781e-113">Verificare che l'applicazione presenti un token di accesso valido a Microsoft Graph come parte della richiesta.</span><span class="sxs-lookup"><span data-stu-id="b781e-113">Ensure that your application is presenting a valid access token to Microsoft Graph as part of the request.</span></span> <span data-ttu-id="b781e-114">Questo errore indica spesso che il token di accesso potrebbe mancare nell'intestazione della richiesta di autenticazione HTTP oppure che il token non è valido o è scaduto.</span><span class="sxs-lookup"><span data-stu-id="b781e-114">This error often means that the access token may be missing in the HTTP authenticate request header or that the token is invalid or has expired.</span></span> <span data-ttu-id="b781e-115">È consigliabile utilizzare la [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) per l'acquisizione dei token di accesso.</span><span class="sxs-lookup"><span data-stu-id="b781e-115">We strongly recommend that you use the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) for access token acquisition.</span></span> <span data-ttu-id="b781e-116">Questo errore può inoltre verificarsi se si tenta di utilizzare un token di accesso delegato concesso a un account Microsoft personale per accedere a un'API che supporta solo gli account di lavoro o dell'Istituto di istruzione (account organizzativi).</span><span class="sxs-lookup"><span data-stu-id="b781e-116">Additionally this error may occur if you try to use a delegated access token granted to a personal Microsoft account to access an API that only supports work or school accounts (organizational accounts).</span></span>

<span data-ttu-id="b781e-117">**403 errore non consentito: si è scelto il set di autorizzazioni appropriato?**</span><span class="sxs-lookup"><span data-stu-id="b781e-117">**403 Forbidden error: Have you chosen the right set of permissions?**</span></span>

<span data-ttu-id="b781e-118">Controllare di aver richiesto il set corretto di autorizzazioni in base alle API di Microsoft Graph chiamate dall'app.</span><span class="sxs-lookup"><span data-stu-id="b781e-118">Check that you have requested the correct set of permissions based on the Microsoft Graph APIs your app calls.</span></span> <span data-ttu-id="b781e-119">Le autorizzazioni meno privilegiate consigliate vengono fornite in tutti gli argomenti del metodo di riferimento dell'API di Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b781e-119">Recommended least privileged permissions are provided in all the Microsoft Graph API reference method topics.</span></span> <span data-ttu-id="b781e-120">Inoltre, tali autorizzazioni devono essere concesse all'applicazione da un utente o da un amministratore.</span><span class="sxs-lookup"><span data-stu-id="b781e-120">Additionally, those permissions must be granted to the application by a user or an administrator.</span></span> <span data-ttu-id="b781e-121">La concessione di autorizzazioni avviene normalmente tramite una pagina di consenso o concedendo le autorizzazioni utilizzando il Blade di registrazione dell'applicazione portale di Azure.</span><span class="sxs-lookup"><span data-stu-id="b781e-121">Granting permissions normally happens through a consent page or by granting permissions using the Azure Portal application registration blade.</span></span> <span data-ttu-id="b781e-122">Dal pannello **Impostazioni** per l'applicazione, fare clic su **autorizzazioni necessarie**, quindi fare clic su **Concedi autorizzazioni**.</span><span class="sxs-lookup"><span data-stu-id="b781e-122">From the **Settings** blade for the application, click **Required Permissions**, and then click **Grant Permissions**.</span></span>

- [<span data-ttu-id="b781e-123">Autorizzazioni di Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b781e-123">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference) 
- [<span data-ttu-id="b781e-124">Informazioni sulle autorizzazioni e sul consenso di Azure AD</span><span class="sxs-lookup"><span data-stu-id="b781e-124">Understanding Azure AD permissions and consent</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

<span data-ttu-id="b781e-125">**403 errore non consentito: l'app ha acquisito un token per soddisfare le autorizzazioni selezionate?**</span><span class="sxs-lookup"><span data-stu-id="b781e-125">**403 Forbidden error: Did your app acquire a token to match chosen permissions?**</span></span>

<span data-ttu-id="b781e-126">Verificare che il tipo di autorizzazioni richieste o concesse corrisponda al tipo di token di accesso acquisito dall'app.</span><span class="sxs-lookup"><span data-stu-id="b781e-126">Make sure that the type of permissions requested or granted matches the type of access token that your app acquires.</span></span> <span data-ttu-id="b781e-127">È possibile che si richiedano e si concessino le autorizzazioni per l'applicazione, ma che si utilizzino token di flusso di codice interattivo delegati invece dei token di flusso di credenziali client o che si richiedano autorizzazioni delegate ma che utilizzino token di flusso di codice delegati.</span><span class="sxs-lookup"><span data-stu-id="b781e-127">You might be requesting and granting application permissions but using delegated interactive code flow tokens instead of client credential flow tokens, or requesting and granting delegated permissions but using client credential flow tokens instead of delegated code flow tokens.</span></span>

- [<span data-ttu-id="b781e-128">Ottenere l'accesso per conto di utenti e autorizzazioni delegate</span><span class="sxs-lookup"><span data-stu-id="b781e-128">Get access on behalf of users and delegated permissions</span></span>](https://docs.microsoft.com/graph/auth_v2_user) 
- [<span data-ttu-id="b781e-129">Flusso del codice di autorizzazione di Azure AD v 2.0-OAuth 2,0</span><span class="sxs-lookup"><span data-stu-id="b781e-129">Azure AD v2.0 - OAuth 2.0 authorization code flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [<span data-ttu-id="b781e-130">Ottenere l'accesso senza un utente (servizio daemon) e le autorizzazioni per l'applicazione</span><span class="sxs-lookup"><span data-stu-id="b781e-130">Get access without a user (daemon service) and application permissions</span></span>](https://docs.microsoft.com/graph/auth_v2_service) 
- [<span data-ttu-id="b781e-131">Flusso delle credenziali client di Azure AD v 2.0-OAuth 2,0</span><span class="sxs-lookup"><span data-stu-id="b781e-131">Azure AD v2.0 - OAuth 2.0 client credentials flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

<span data-ttu-id="b781e-132">**403 errore non consentito: reimpostazione della password**</span><span class="sxs-lookup"><span data-stu-id="b781e-132">**403 Forbidden error: Resetting password**</span></span>

<span data-ttu-id="b781e-133">Attualmente, non sono disponibili autorizzazioni di servizio per il daemon di autorizzazioni per l'applicazione che consentono di reimpostare le password degli utenti.</span><span class="sxs-lookup"><span data-stu-id="b781e-133">Currently, there are no application permission daemon service-to-service permissions that allow resetting user passwords.</span></span> <span data-ttu-id="b781e-134">Queste API sono supportate solo mediante flussi di codice delegati interattivi con un amministratore connesso.</span><span class="sxs-lookup"><span data-stu-id="b781e-134">These APIs are only supported using the interactive delegated code flows with a signed-in administrator.</span></span>

- [<span data-ttu-id="b781e-135">Autorizzazioni di Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b781e-135">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference)

<span data-ttu-id="b781e-136">**403 Forbidden: l'utente ha accesso e ha una licenza?**</span><span class="sxs-lookup"><span data-stu-id="b781e-136">**403 Forbidden: Does the user have access and are they licensed?**</span></span>

<span data-ttu-id="b781e-137">Per i flussi di codice delegati, Microsoft Graph valuta se la richiesta è consentita in base alle autorizzazioni concesse all'app e alle autorizzazioni che l'utente ha eseguito l'accesso.</span><span class="sxs-lookup"><span data-stu-id="b781e-137">For delegated code flows, Microsoft Graph evaluates if the request is allowed based on the permissions granted to the app and the permissions that the signed-in user has.</span></span> <span data-ttu-id="b781e-138">In genere, questo errore indica che l'utente non è sufficientemente privilegiato per eseguire la richiesta o che l'utente non dispone di una licenza per i dati a cui si accede.</span><span class="sxs-lookup"><span data-stu-id="b781e-138">Generally, this error indicates that the user is not privileged enough to perform the request or the user is not licensed for the data being accessed.</span></span> <span data-ttu-id="b781e-139">Solo gli utenti che dispongono delle autorizzazioni o delle licenze necessarie possono eseguire correttamente la richiesta.</span><span class="sxs-lookup"><span data-stu-id="b781e-139">Only users with the required permissions or licenses can make the request successfully.</span></span>

<span data-ttu-id="b781e-140">**403 Forbidden: è stata selezionata l'API delle risorse corretta?**</span><span class="sxs-lookup"><span data-stu-id="b781e-140">**403 Forbidden: Did you select the correct resource API?**</span></span>

<span data-ttu-id="b781e-141">I servizi API come Microsoft Graph verificano che l'attestazione AUD (gruppo di destinatari) nel token di accesso ricevuto corrisponda al valore previsto per se stesso e, in caso contrario, genera un errore 403 Forbidden.</span><span class="sxs-lookup"><span data-stu-id="b781e-141">API services like Microsoft Graph check that the aud claim (audience) in the received access token matches the value it expects for itself, and if not, it results in a 403 Forbidden error.</span></span> <span data-ttu-id="b781e-142">Un errore comune risultante da questo errore consiste nel tentativo di utilizzare un token acquisito per API di Azure AD Graph, API di Outlook o API di SharePoint/OneDrive per chiamare Microsoft Graph (o viceversa).</span><span class="sxs-lookup"><span data-stu-id="b781e-142">A common mistake resulting in this error is trying to use a token acquired for Azure AD Graph APIs, Outlook APIs, or SharePoint/OneDrive APIs to call Microsoft Graph (or vice versa).</span></span> <span data-ttu-id="b781e-143">Verificare che la risorsa (o ambito) dell'app acquisisca un token per la corrispondenza con l'API chiamata dall'app.</span><span class="sxs-lookup"><span data-stu-id="b781e-143">Ensure that the resource (or scope) your app is acquiring a token for matches the API that the app is calling.</span></span>

<span data-ttu-id="b781e-144">**400 Bad Request o 403 Forbidden: l'utente è conforme ai criteri di accesso condizionale (CA) dell'organizzazione?**</span><span class="sxs-lookup"><span data-stu-id="b781e-144">**400 Bad Request or 403 Forbidden: Does the user comply with their organization's conditional access (CA) policies?**</span></span>

<span data-ttu-id="b781e-145">In base ai criteri della CA dell'organizzazione, un utente che accede alle risorse di Microsoft Graph tramite l'app può essere messo in discussione per ulteriori informazioni che non sono presenti nel token di accesso acquistato originariamente dall'app.</span><span class="sxs-lookup"><span data-stu-id="b781e-145">Based on an organization's CA policies, a user accessing Microsoft Graph resources via your app may be challenged for additional information that is not present in the access token your app originally acquired.</span></span> <span data-ttu-id="b781e-146">In questo caso, l'app riceve un 400 con un *interaction_required* errore durante l'acquisizione di un token di accesso o un 403 con *insufficient_claims* errore durante la chiamata a Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b781e-146">In this case, your app receives a 400 with an *interaction_required* error during access token acquisition or a 403 with *insufficient_claims* error when calling Microsoft Graph.</span></span> <span data-ttu-id="b781e-147">In entrambi i casi, la risposta di errore contiene informazioni aggiuntive che possono essere presentate all'endpoint autorizza per contestare l'utente per ulteriori informazioni, ad esempio l'autenticazione a più fattori o la registrazione dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="b781e-147">In both cases, the error response contains additional information that can be presented to the authorize endpoint to challenge the user for additional information (like multi-factor authentication or device enrollment).</span></span>

- [<span data-ttu-id="b781e-148">Gestione delle sfide di accesso condizionale tramite MSAL </span><span class="sxs-lookup"><span data-stu-id="b781e-148">Handling conditional access challenges using MSAL </span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [<span data-ttu-id="b781e-149">Guida per gli sviluppatori per l'accesso condizionale di Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="b781e-149">Developer guidance for Azure Active Directory conditional access</span></span>](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)