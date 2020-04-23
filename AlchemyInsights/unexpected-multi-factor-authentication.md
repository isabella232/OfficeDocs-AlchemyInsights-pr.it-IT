---
title: Autenticazione a più fattori imprevista
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: a664bd709062ec1335ebcf1f9adddc8aef917ac1
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766605"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="e7700-102">Autenticazione a più fattori imprevista</span><span class="sxs-lookup"><span data-stu-id="e7700-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="e7700-103">Se il tenant è stato creato dopo il 21 ottobre 2019 e si riceve una richiesta di conferma per l'autenticazione a più fattori, è probabile che siano state abilitate le [impostazioni predefinite per la sicurezza](https://aka.ms/securitydefaults) nel tenant.</span><span class="sxs-lookup"><span data-stu-id="e7700-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="e7700-104">Per gestire le impostazioni predefinite per la sicurezza:</span><span class="sxs-lookup"><span data-stu-id="e7700-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="e7700-105">Accedere all'[interfaccia di amministrazione](https://go.microsoft.com/fwlink/p/?linkid=834822) con le credenziali di amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="e7700-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="e7700-106">Passare alle [Proprietà di Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="e7700-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="e7700-107">Nella parte inferiore della pagina fare clic su **Gestire le impostazioni predefinite per la sicurezza**.</span><span class="sxs-lookup"><span data-stu-id="e7700-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="e7700-108">Fare clic su **Sì** per abilitare le impostazioni predefinite di sicurezza e su **No** per disabilitare le impostazioni predefinite per la sicurezza.</span><span class="sxs-lookup"><span data-stu-id="e7700-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
