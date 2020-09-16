---
title: Autenticazione a più fattori imprevista
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 48303d5b408cbdb243ec45dc4c80ac9a83f273a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689526"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="983f3-102">Autenticazione a più fattori imprevista</span><span class="sxs-lookup"><span data-stu-id="983f3-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="983f3-103">Se il tenant è stato creato dopo il 21 ottobre 2019 e si riceve una richiesta di conferma per l'autenticazione a più fattori, è probabile che siano state abilitate le [impostazioni predefinite per la sicurezza](https://aka.ms/securitydefaults) nel tenant.</span><span class="sxs-lookup"><span data-stu-id="983f3-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="983f3-104">Per gestire le impostazioni predefinite per la sicurezza:</span><span class="sxs-lookup"><span data-stu-id="983f3-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="983f3-105">Accedere all'[interfaccia di amministrazione](https://go.microsoft.com/fwlink/p/?linkid=834822) con le credenziali di amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="983f3-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="983f3-106">Passare alle [Proprietà di Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="983f3-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="983f3-107">Nella parte inferiore della pagina fare clic su **Gestire le impostazioni predefinite per la sicurezza**.</span><span class="sxs-lookup"><span data-stu-id="983f3-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="983f3-108">Fare clic su **Sì** per abilitare le impostazioni predefinite di sicurezza e su **No** per disabilitare le impostazioni predefinite per la sicurezza.</span><span class="sxs-lookup"><span data-stu-id="983f3-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
