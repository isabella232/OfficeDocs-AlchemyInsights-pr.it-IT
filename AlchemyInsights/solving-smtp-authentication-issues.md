---
title: Risolvere i problemi di autenticazione SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264434"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="15c92-102">Risolvere i problemi di autenticazione SMTP</span><span class="sxs-lookup"><span data-stu-id="15c92-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="15c92-103">Se si verificano gli errori 5.7.57 o 5.7.3 quando si prova a inviare posta elettronica SMTP ed eseguire l'autenticazione con un client o un'applicazione, è necessario verificare alcuni aspetti:</span><span class="sxs-lookup"><span data-stu-id="15c92-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="15c92-104">L'invio SMTP autenticato potrebbe essere disabilitato nel tenant o nella cassetta postale che si sta provando a usare (controllare entrambe le impostazioni).</span><span class="sxs-lookup"><span data-stu-id="15c92-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="15c92-105">Per altre informazioni, vedere [Abilitare o disabilitare l'invio SMTP client autenticato](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="15c92-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="15c92-106">Controllare se per il tenant sono abilitate le [Impostazioni predefinite per la sicurezza di Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). Se abilitate, l'autenticazione SMTP mediante autenticazione di base, nota anche come legacy, che usa il nome utente e la password, non riuscirà.</span><span class="sxs-lookup"><span data-stu-id="15c92-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
