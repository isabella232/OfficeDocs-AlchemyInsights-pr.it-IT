---
title: Problemi con MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810488"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="608e7-102">Problemi con Azure MFA</span><span class="sxs-lookup"><span data-stu-id="608e7-102">Issues with Azure MFA</span></span>
<span data-ttu-id="608e7-103">Ci sono un paio di cose da verificare se gli utenti non possono accedere usando l'autenticazione a più fattori (MFA)</span><span class="sxs-lookup"><span data-stu-id="608e7-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="608e7-104">L'utente interessato potrebbe essere bloccato nel portale di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="608e7-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="608e7-105">In questo caso, i tentativi di autenticazione per l'utente specifico verranno automaticamente negati.</span><span class="sxs-lookup"><span data-stu-id="608e7-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="608e7-106">Segui i passaggi descritti in questo articolo per sbloccarli.</span><span class="sxs-lookup"><span data-stu-id="608e7-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="608e7-107">Se lo sblocco dell'utente non è stato utile o l'utente non è bloccato, puoi provare a reimpostare la MFA per l'utente e l'utente dovrà ripetere il processo di registrazione.</span><span class="sxs-lookup"><span data-stu-id="608e7-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="608e7-108">Seguire i passaggi descritti in questo articolo.</span><span class="sxs-lookup"><span data-stu-id="608e7-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="608e7-109">Se questa è la prima volta che hai abilitato L'autenticazione a più fattori e gli utenti non sono in grado di accedere a client non browser come Outlook, Skype e così via, ad esempio ADAL (Active Directory Authentication Library) non è abilitato nell'abbonamento a O365.</span><span class="sxs-lookup"><span data-stu-id="608e7-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="608e7-110">In questo caso sarà necessario connettersi a PowerShell di Exchange Online ed eseguire questo cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="608e7-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>