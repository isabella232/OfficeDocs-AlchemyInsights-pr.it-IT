---
title: Non è possibile accedere alle cartelle pubbliche
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812551"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="bdc6e-102">Outlook non è in grado di connettersi alle cartelle pubbliche</span><span class="sxs-lookup"><span data-stu-id="bdc6e-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="bdc6e-103">Se l'accesso alle cartelle pubbliche non funziona per alcuni utenti, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="bdc6e-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="bdc6e-104">Connettersi a EXO PowerShell e configurare il parametro DefaultPublicFolderMailbox nell'account utente problema in modo che corrisponda al parametro su un account utente funzionante.</span><span class="sxs-lookup"><span data-stu-id="bdc6e-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="bdc6e-105">Esempio:</span><span class="sxs-lookup"><span data-stu-id="bdc6e-105">Example:</span></span>

<span data-ttu-id="bdc6e-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="bdc6e-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="bdc6e-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="bdc6e-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="bdc6e-108">Attendere almeno un'ora per rendere effettive le modifiche.</span><span class="sxs-lookup"><span data-stu-id="bdc6e-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="bdc6e-109">Se il problema persiste, eseguire la [procedura seguente](https://aka.ms/pfcte) per risolvere i problemi di accesso alle cartelle pubbliche con Outlook.</span><span class="sxs-lookup"><span data-stu-id="bdc6e-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="bdc6e-110">**Per controllare quali utenti possono accedere alle cartelle pubbliche con Outlook**:</span><span class="sxs-lookup"><span data-stu-id="bdc6e-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="bdc6e-111">Utilizzare Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true o $false</span><span class="sxs-lookup"><span data-stu-id="bdc6e-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="bdc6e-112">$true: consente agli utenti di accedere alle cartelle pubbliche in Outlook</span><span class="sxs-lookup"><span data-stu-id="bdc6e-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="bdc6e-113">$false: consente agli utenti di accedere alle cartelle pubbliche in Outlook. </span><span class="sxs-lookup"><span data-stu-id="bdc6e-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="bdc6e-114">Questo è il valore predefinito.</span><span class="sxs-lookup"><span data-stu-id="bdc6e-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="bdc6e-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="bdc6e-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="bdc6e-116">**Note** Questa procedura consente di controllare le connessioni solo con i client di Outlook desktop per Windows.</span><span class="sxs-lookup"><span data-stu-id="bdc6e-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="bdc6e-117">Un utente può continuare ad accedere alle cartelle pubbliche utilizzando OWA o Outlook per Mac.</span><span class="sxs-lookup"><span data-stu-id="bdc6e-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="bdc6e-118">Per altre informazioni, vedere [annuncio del supporto per le connessioni controllate alle cartelle pubbliche in Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="bdc6e-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>