---
title: Errore durante la convalida del token di accesso durante l'on-boarding di Desktop Analytics
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813692"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="ebe4c-102">Errore "Errore durante la convalida del token di accesso" durante l'onboarding di Desktop Analytics</span><span class="sxs-lookup"><span data-stu-id="ebe4c-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="ebe4c-103">Questo errore viene in genere rilevato alla scadenza del token di autenticazione.</span><span class="sxs-lookup"><span data-stu-id="ebe4c-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="ebe4c-104">In genere, l'aggiornamento della pagina aggiorna il token.</span><span class="sxs-lookup"><span data-stu-id="ebe4c-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="ebe4c-105">Tuttavia, questo problema può persistere se all'account utilizzato per l'on-board Desktop Analytics sono applicati criteri di accesso condizionale.</span><span class="sxs-lookup"><span data-stu-id="ebe4c-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="ebe4c-106">È possibile esaminare i log di accesso di Azure AD nel portale di Azure per verificare se sono presenti errori di accesso per l'account utilizzato per l'onboarding di Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="ebe4c-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="ebe4c-107">Per ulteriori informazioni sull'accesso condizionale, vedere [Plan your Conditional Access deployment.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="ebe4c-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>