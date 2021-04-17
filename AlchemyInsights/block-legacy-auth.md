---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820182"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="2cf52-102">Blocco dell'autenticazione legacy</span><span class="sxs-lookup"><span data-stu-id="2cf52-102">Blocking legacy authentication</span></span>

<span data-ttu-id="2cf52-103">Con il termine autenticazione legacy si fa riferimento a una richiesta di autenticazione effettuata da:</span><span class="sxs-lookup"><span data-stu-id="2cf52-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="2cf52-104">Client di Office meno recenti che non utilizzano l'autenticazione moderna (ad esempio, client di Office 2010).</span><span class="sxs-lookup"><span data-stu-id="2cf52-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="2cf52-105">Qualsiasi client che usi protocolli di posta elettronica legacy come IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="2cf52-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="2cf52-106">Per ulteriori informazioni sul blocco dell'autenticazione legacy e sull'abilitazione dell'autenticazione [moderna,](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)vedere Blocking legacy authentication .</span><span class="sxs-lookup"><span data-stu-id="2cf52-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="2cf52-107">Le impostazioni predefinite di sicurezza in Azure Active Directory (Azure AD) semplificano la protezione e consentono di proteggere l'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="2cf52-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="2cf52-108">Le impostazioni predefinite di sicurezza contengono impostazioni di sicurezza preconfigurate per gli attacchi comuni.</span><span class="sxs-lookup"><span data-stu-id="2cf52-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="2cf52-109">Per ulteriori informazioni sulle impostazioni predefinite di sicurezza, vedere [Che cosa sono le impostazioni predefinite di sicurezza?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="2cf52-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="2cf52-110">**Nota:** se il tenant è stato creato il 22 ottobre 2019 o dopo il 22 ottobre 2019, è possibile che si verifichi il nuovo comportamento di protezione per impostazione predefinita e che siano già abilitate le impostazioni predefinite di sicurezza nel tenant.</span><span class="sxs-lookup"><span data-stu-id="2cf52-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="2cf52-111">Per proteggere tutti gli utenti, le impostazioni predefinite di sicurezza vengono implementare in tutti i nuovi tenant creati.</span><span class="sxs-lookup"><span data-stu-id="2cf52-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
