---
title: Non è possibile accedere alle cartelle pubbliche
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891753"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="9f6eb-102">Outlook non è in grado di connettersi alle cartelle pubbliche</span><span class="sxs-lookup"><span data-stu-id="9f6eb-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="9f6eb-103">Se l'accesso alle cartelle pubbliche non funziona per alcuni utenti, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="9f6eb-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="9f6eb-104">Connettersi a EXO PowerShell e configurare il parametro DefaultPublicFolderMailbox nell'account utente problema in modo che corrisponda al parametro su un account utente funzionante.</span><span class="sxs-lookup"><span data-stu-id="9f6eb-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="9f6eb-105">Esempio:</span><span class="sxs-lookup"><span data-stu-id="9f6eb-105">Example:</span></span>

<span data-ttu-id="9f6eb-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="9f6eb-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="9f6eb-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<valore dal comando precedente></span><span class="sxs-lookup"><span data-stu-id="9f6eb-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="9f6eb-108">Attendere almeno un'ora per rendere effettive le modifiche.</span><span class="sxs-lookup"><span data-stu-id="9f6eb-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="9f6eb-109">Se il problema persiste, eseguire la [procedura seguente](https://aka.ms/pfcte) per risolvere i problemi di accesso alle cartelle pubbliche con Outlook.</span><span class="sxs-lookup"><span data-stu-id="9f6eb-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>