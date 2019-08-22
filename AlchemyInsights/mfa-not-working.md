---
title: Problemi con AMF
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545173"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="e5f3d-102">Problemi con AMF</span><span class="sxs-lookup"><span data-stu-id="e5f3d-102">Issues with MFA</span></span>
<span data-ttu-id="e5f3d-103">Ci sono un paio di cose da controllare se gli utenti non possono accedere utilizzando l'autenticazione a più fattori (AMF)</span><span class="sxs-lookup"><span data-stu-id="e5f3d-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="e5f3d-104">L'utente può essere bloccato nel portale di Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e5f3d-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="e5f3d-105">In caso contrario, i tentativi di autenticazione per l'utente specifico verranno negati automaticamente.</span><span class="sxs-lookup"><span data-stu-id="e5f3d-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="e5f3d-106">Attenersi alla procedura descritta in questo articolo per sbloccarli.</span><span class="sxs-lookup"><span data-stu-id="e5f3d-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="e5f3d-107">Se lo sblocco dell'utente non è stato di aiuto o se l'utente non è bloccato, è possibile provare a reimpostare AMF per l'utente e il processo di registrazione passerà di nuovo.</span><span class="sxs-lookup"><span data-stu-id="e5f3d-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="e5f3d-108">Seguire le istruzioni riportate in questo articolo.</span><span class="sxs-lookup"><span data-stu-id="e5f3d-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="e5f3d-109">Se è la prima volta che si Abilita l'autenticazione master e gli utenti non sono in grado di accedere ai client non browser come Outlook, Skype e così via, è possibile che ADAL (Active Directory Authentication Library) non sia abilitato per l'abbonamento a O365.</span><span class="sxs-lookup"><span data-stu-id="e5f3d-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="e5f3d-110">In questo caso, sarà necessario connettersi a PowerShell di Exchange Online ed eseguire questo cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="e5f3d-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>