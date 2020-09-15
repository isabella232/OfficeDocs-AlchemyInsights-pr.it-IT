---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685602"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="d9a19-102">Blocco dell'autenticazione legacy</span><span class="sxs-lookup"><span data-stu-id="d9a19-102">Blocking legacy authentication</span></span>

<span data-ttu-id="d9a19-103">Con il termine autenticazione legacy si fa riferimento a una richiesta di autenticazione effettuata da:</span><span class="sxs-lookup"><span data-stu-id="d9a19-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="d9a19-104">Client di Office meno recenti che non utilizzano l'autenticazione moderna (ad esempio, il client di Office 2010).</span><span class="sxs-lookup"><span data-stu-id="d9a19-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="d9a19-105">Qualsiasi client che usi protocolli di posta elettronica legacy come IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="d9a19-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="d9a19-106">Per ulteriori informazioni sul blocco dell'autenticazione legacy e sull'abilitazione dell'autenticazione moderna, vedere [Blocking legacy Authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="d9a19-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="d9a19-107">Per le impostazioni predefinite di sicurezza in Azure Active Directory (Azure AD), è più facile essere sicuri e proteggere l'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="d9a19-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="d9a19-108">Le impostazioni predefinite per la sicurezza contengono preconfigured Security Settings for Common attacks.</span><span class="sxs-lookup"><span data-stu-id="d9a19-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="d9a19-109">Per ulteriori informazioni sulle impostazioni predefinite per la sicurezza, fare riferimento a [quali sono le impostazioni predefinite per la sicurezza?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="d9a19-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="d9a19-110">**Nota**: se il tenant è stato creato il 22 ottobre 2019, è possibile che si verifichi il nuovo comportamento sicuro per impostazione predefinita e che siano già attivate le impostazioni predefinite per la sicurezza nel tenant.</span><span class="sxs-lookup"><span data-stu-id="d9a19-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="d9a19-111">Per proteggere tutti gli utenti, le impostazioni predefinite per la sicurezza vengono distribuite a tutti i nuovi tenant creati.</span><span class="sxs-lookup"><span data-stu-id="d9a19-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
