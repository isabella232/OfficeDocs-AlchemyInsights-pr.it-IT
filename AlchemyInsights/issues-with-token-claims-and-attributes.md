---
title: Problemi relativi alle attestazioni e agli attributi dei token
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029988"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="2e7e3-102">Problemi relativi alle attestazioni e agli attributi dei token</span><span class="sxs-lookup"><span data-stu-id="2e7e3-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="2e7e3-103">**Update, Configure or Remove token Claims**</span><span class="sxs-lookup"><span data-stu-id="2e7e3-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="2e7e3-104">Utilizzando Azure Active Directory (Azure AD), è possibile [personalizzare il tipo di attestazione per l'attestazione di ruolo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) nel token di risposta visualizzato dopo l'autorizzazione di un'app.</span><span class="sxs-lookup"><span data-stu-id="2e7e3-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="2e7e3-105">Gli sviluppatori di applicazioni possono utilizzare attestazioni facoltative nelle applicazioni di Azure AD per specificare le attestazioni desiderate nei token inviati all'applicazione.</span><span class="sxs-lookup"><span data-stu-id="2e7e3-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="2e7e3-106">Per ulteriori informazioni, vedere [fornire attestazioni facoltative per l'app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="2e7e3-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="2e7e3-107">[Configurare le attestazioni di gruppo per le applicazioni con Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="2e7e3-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="2e7e3-108">Se si utilizza l'accesso Single Sign-on senza problemi nell'applicazione, vedere [Customize Claims issued nel token SAML for Enterprise Applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="2e7e3-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="2e7e3-109">**Mapping degli attributi delle attestazioni**</span><span class="sxs-lookup"><span data-stu-id="2e7e3-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="2e7e3-110">Per configurare i criteri di mapping delle attestazioni tramite PowerShell, vedere [Customize Claims emitted in Tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="2e7e3-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="2e7e3-111">Gli attributi di estensione dello schema di directory consentono di archiviare dati aggiuntivi in Azure Active Directory per gli oggetti utente e altri oggetti directory, ad esempio gruppi, dettagli tenant, entità di servizio.</span><span class="sxs-lookup"><span data-stu-id="2e7e3-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="2e7e3-112">Solo gli attributi di estensione per gli oggetti utente possono essere utilizzati per la creazione di attestazioni per le applicazioni.</span><span class="sxs-lookup"><span data-stu-id="2e7e3-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="2e7e3-113">[Using Directory Schema Extension Attributes in Claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) descrive come utilizzare gli attributi di estensione dello schema di directory per l'invio dei dati degli utenti alle applicazioni in attestazioni di token.</span><span class="sxs-lookup"><span data-stu-id="2e7e3-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="2e7e3-114">Per ulteriori informazioni sulle attestazioni dei token, vedere:</span><span class="sxs-lookup"><span data-stu-id="2e7e3-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="2e7e3-115">Attestazioni nei token di accesso</span><span class="sxs-lookup"><span data-stu-id="2e7e3-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="2e7e3-116">Attestazioni in un id_token</span><span class="sxs-lookup"><span data-stu-id="2e7e3-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="2e7e3-117">[Attestazioni](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) che è possibile prevedere nei token di ID e nei token di accesso emessi da Azure ad B2C</span><span class="sxs-lookup"><span data-stu-id="2e7e3-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="2e7e3-118">Riferimento per le attestazioni di token SAML</span><span class="sxs-lookup"><span data-stu-id="2e7e3-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
