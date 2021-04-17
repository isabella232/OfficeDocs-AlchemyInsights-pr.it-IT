---
title: Criteri di accesso condizionale
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817284"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="d1fd2-102">Criteri di accesso condizionale</span><span class="sxs-lookup"><span data-stu-id="d1fd2-102">Conditional Access policies</span></span>

<span data-ttu-id="d1fd2-103">L'accesso condizionale è una funzionalità di Azure AD che consente di imporre controlli sull'accesso alle app nell'ambiente, in base a condizioni specifiche e gestiti da una posizione centrale.</span><span class="sxs-lookup"><span data-stu-id="d1fd2-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="d1fd2-104">Leggere altre informazioni sull'[Accesso condizionale di Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="d1fd2-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="d1fd2-105">**Nota**: se il tenant è stato creato dopo il 21 ottobre 2019 e si riceve una richiesta di conferma per l'autenticazione a più fattori, è probabile che siano state abilitate le [impostazioni predefinite per la sicurezza nel tenant](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="d1fd2-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="d1fd2-106">**Per gestire le impostazioni predefinite per la sicurezza**</span><span class="sxs-lookup"><span data-stu-id="d1fd2-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="d1fd2-107">Accedere all'[interfaccia di amministrazione](https://go.microsoft.com/fwlink/p/?linkid=834822) con le credenziali di amministratore globale.</span><span class="sxs-lookup"><span data-stu-id="d1fd2-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="d1fd2-108">Passare alle [Proprietà di Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="d1fd2-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="d1fd2-109">Nella parte inferiore della pagina fare clic su **Gestire le impostazioni predefinite per la sicurezza**.</span><span class="sxs-lookup"><span data-stu-id="d1fd2-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="d1fd2-110">Fare clic su **Sì** per abilitare le impostazioni predefinite di sicurezza o su **No** per disabilitare le impostazioni predefinite per la sicurezza.</span><span class="sxs-lookup"><span data-stu-id="d1fd2-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
