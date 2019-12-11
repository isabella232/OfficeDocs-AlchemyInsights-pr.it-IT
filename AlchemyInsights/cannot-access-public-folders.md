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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959499"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="31190-102">Outlook non è in grado di connettersi alle cartelle pubbliche</span><span class="sxs-lookup"><span data-stu-id="31190-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="31190-103">Se l'accesso alle cartelle pubbliche non funziona per alcuni utenti, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="31190-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="31190-104">Connettersi a EXO PowerShell e configurare DefaultPublicFolderMailbox nell'account utente del problema in modo che corrisponda a uno su un account utente funzionante.</span><span class="sxs-lookup"><span data-stu-id="31190-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="31190-105">Esempio:</span><span class="sxs-lookup"><span data-stu-id="31190-105">Example:</span></span>

<span data-ttu-id="31190-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="31190-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="31190-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<valore dal comando precedente></span><span class="sxs-lookup"><span data-stu-id="31190-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="31190-108">Attendere almeno un'ora per rendere effettive le modifiche.</span><span class="sxs-lookup"><span data-stu-id="31190-108">Wait at least one hour for the change to take effect.</span></span>