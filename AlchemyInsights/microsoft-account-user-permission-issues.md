---
title: Risoluzione dei problemi relativi a un utente non trovato nella directory
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702742"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="abe48-102">Risoluzione dei problemi relativi a un utente non trovato nella directory</span><span class="sxs-lookup"><span data-stu-id="abe48-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="abe48-103">Se gli utenti ricevono il messaggio di errore "l'utente non può essere trovato" nella directory, provare di nuovo in cui il tipo di problema è utente non presente nella directory.</span><span class="sxs-lookup"><span data-stu-id="abe48-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="abe48-104">Per risolvere il problema, è possibile completare i passaggi seguenti.</span><span class="sxs-lookup"><span data-stu-id="abe48-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="abe48-105">Verificare che l'account che ha accettato l'invito alla posta elettronica sia lo stesso utilizzato per l'accesso in un secondo momento.</span><span class="sxs-lookup"><span data-stu-id="abe48-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="abe48-106">Assicurarsi che l'utente stia utilizzando lo stesso account per accettare l'invito e accedere al sito.</span><span class="sxs-lookup"><span data-stu-id="abe48-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="abe48-107">Per altre informazioni, vedere [How to Manage aliases for your Microsoft</a> account to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="abe48-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="abe48-108">Passare a ogni sito o i siti in cui l'utente riceve l'errore.</span><span class="sxs-lookup"><span data-stu-id="abe48-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="abe48-109">Aggiungere "/_layouts/15/people.aspx/membershipgroupid = 0" (tra virgolette doppie) alla fine dell'URL del sito.</span><span class="sxs-lookup"><span data-stu-id="abe48-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="abe48-110">Esempio: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="abe48-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="abe48-111">Selezionare l'utente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="abe48-111">Select the user from the list.</span></span>

- <span data-ttu-id="abe48-112">Fare clic su **Rimuovi autorizzazioni utente** dalla barra multifunzione.</span><span class="sxs-lookup"><span data-stu-id="abe48-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="abe48-113">Aggiungere di nuovo l'utente e rinviare l'invito all'utente.</span><span class="sxs-lookup"><span data-stu-id="abe48-113">Add back the User and Resend the invite to the user.</span></span>

