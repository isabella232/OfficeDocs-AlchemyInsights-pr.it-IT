---
title: Configurare ed estendere la durata dei token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/20/2021
ms.locfileid: "49911997"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="45e0e-102">Configurare ed estendere la durata dei token</span><span class="sxs-lookup"><span data-stu-id="45e0e-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="45e0e-103">È possibile specificare la durata di token di accesso, SAML o ID emesso da Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="45e0e-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="45e0e-104">Inoltre, è possibile impostare la durata dei token per tutte le app dell'organizzazione, per un'applicazione multi-tenant (più organizzazioni) o per un'entità servizio specifica all'interno dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="45e0e-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="45e0e-105">Per altre informazioni, leggere [Durata dei token configurabile](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="45e0e-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="45e0e-106">Per esempi, leggere [Esempi su come configurare la durata del token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="45e0e-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="45e0e-107">Per informazioni su come configurare la durata e la compatibilità di un token in Azure Active Directory B2C (Azure AD B2C), vedere [Configurare token in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="45e0e-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="45e0e-108">L'articolo [Configurare il comportamento della sessione in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) descrive i metodi Single Sign-On (SSO) usati in Azure AD B2C e consente di scegliere il metodo SSO più appropriato per la configurazione dei criteri.</span><span class="sxs-lookup"><span data-stu-id="45e0e-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="45e0e-109">**Qual è la durata di un token? Per quanto tempo è valido?**</span><span class="sxs-lookup"><span data-stu-id="45e0e-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="45e0e-110">La durata di un token è di 1 ora, la durata di una sessione è di 24 ore.</span><span class="sxs-lookup"><span data-stu-id="45e0e-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="45e0e-111">Ciò significa che se non vengono inviate richieste entro 24 ore, sarà necessario accedere di nuovo prima di richiedere un nuovo token.</span><span class="sxs-lookup"><span data-stu-id="45e0e-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="45e0e-112">A partire dal 30 maggio 2020, nessun nuovo tenant può usare i criteri di durata dei token configurabile per impostare i token della sessione e di aggiornamento.</span><span class="sxs-lookup"><span data-stu-id="45e0e-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="45e0e-113">La deprecazione avverrà in diversi mesi, ciò significa che non verranno più rispettati i criteri dei token di sessione e di aggiornamento esistenti.</span><span class="sxs-lookup"><span data-stu-id="45e0e-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="45e0e-114">È comunque possibile configurare la durata del token di accesso dopo la deprecazione.</span><span class="sxs-lookup"><span data-stu-id="45e0e-114">You can still configure access token lifetimes after the deprecation.</span></span>






