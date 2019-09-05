---
title: Risoluzione dei problemi relativi a un utente non trovato nella directory
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754196"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="664ef-102">Risoluzione dei problemi relativi a un utente non trovato nella directory</span><span class="sxs-lookup"><span data-stu-id="664ef-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="664ef-103">Se gli utenti ricevono il messaggio di errore "l'utente non può essere trovato" nella directory.</span><span class="sxs-lookup"><span data-stu-id="664ef-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="664ef-104">Provare di nuovo in cui il tipo di problema è utente non presente nella directory.</span><span class="sxs-lookup"><span data-stu-id="664ef-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="664ef-105">Per risolvere il problema, è possibile completare i passaggi seguenti.</span><span class="sxs-lookup"><span data-stu-id="664ef-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="664ef-106">Verificare che l'account che ha accettato l'invito alla posta elettronica sia lo stesso utilizzato per l'accesso in un secondo momento.</span><span class="sxs-lookup"><span data-stu-id="664ef-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="664ef-107">Assicurarsi che l'utente stia utilizzando lo stesso account per accettare l'invito e accedere al sito.</span><span class="sxs-lookup"><span data-stu-id="664ef-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="664ef-108">Per altre informazioni, vedere [How to Manage aliases for your Microsoft</a> account to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="664ef-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="664ef-109">Passare a ogni sito o i siti in cui l'utente riceve l'errore.</span><span class="sxs-lookup"><span data-stu-id="664ef-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="664ef-110">Aggiungere "/_layouts/15/people.aspx/membershipgroupid = 0" (tra virgolette doppie) alla fine dell'URL del sito.</span><span class="sxs-lookup"><span data-stu-id="664ef-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="664ef-111">Esempio: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="664ef-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="664ef-112">Selezionare l'utente dall'elenco.</span><span class="sxs-lookup"><span data-stu-id="664ef-112">Select the user from the list.</span></span>

- <span data-ttu-id="664ef-113">Fare clic su **Rimuovi autorizzazioni utente** dalla barra multifunzione.</span><span class="sxs-lookup"><span data-stu-id="664ef-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="664ef-114">Aggiungere di nuovo l'utente e rinviare l'invito all'utente.</span><span class="sxs-lookup"><span data-stu-id="664ef-114">Add back the User and Resend the invite to the user.</span></span>

