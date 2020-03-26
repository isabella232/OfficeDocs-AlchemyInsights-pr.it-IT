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
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946741"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="ee55d-102">Autenticazione a più fattori imprevista</span><span class="sxs-lookup"><span data-stu-id="ee55d-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="ee55d-103">Se il tenant è stato creato dopo il 21 ottobre 2019 e si riceve una richiesta di conferma per l'autenticazione a più fattori, è probabile che siano state abilitate le [impostazioni predefinite per la sicurezza](http://aka.ms/securitydefaults) nel tenant.</span><span class="sxs-lookup"><span data-stu-id="ee55d-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="ee55d-104">Per gestire le impostazioni predefinite per la sicurezza:</span><span class="sxs-lookup"><span data-stu-id="ee55d-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="ee55d-105">Accedere all'[interfaccia di amministrazione](https://go.microsoft.com/fwlink/p/?linkid=834822) con le credenziali di amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="ee55d-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="ee55d-106">Passare alle [Proprietà di Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="ee55d-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="ee55d-107">Nella parte inferiore della pagina fare clic su **Gestire le impostazioni predefinite per la sicurezza**.</span><span class="sxs-lookup"><span data-stu-id="ee55d-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="ee55d-108">Fare clic su **Sì** per abilitare le impostazioni predefinite di sicurezza e su **No** per disabilitare le impostazioni predefinite per la sicurezza.</span><span class="sxs-lookup"><span data-stu-id="ee55d-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
