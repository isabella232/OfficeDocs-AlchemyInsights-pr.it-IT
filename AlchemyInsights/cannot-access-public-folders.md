---
title: Impossibile accedere alle cartelle pubbliche
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819516"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="a7e8d-102">Outlook non è in grado di connettersi alle cartelle pubbliche</span><span class="sxs-lookup"><span data-stu-id="a7e8d-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="a7e8d-103">Se l'accesso alle cartelle pubbliche non funziona per alcuni utenti, provare a eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="a7e8d-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="a7e8d-104">Connettersi a EXO PowerShell e configurare il parametro DefaultPublicFolderMailbox nell'account utente problematico in modo che corrisponda al parametro in un account utente funzionante.</span><span class="sxs-lookup"><span data-stu-id="a7e8d-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="a7e8d-105">Esempio:</span><span class="sxs-lookup"><span data-stu-id="a7e8d-105">Example:</span></span>

<span data-ttu-id="a7e8d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="a7e8d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="a7e8d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="a7e8d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="a7e8d-108">Attendere almeno un'ora per l'applicazione della modifica.</span><span class="sxs-lookup"><span data-stu-id="a7e8d-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="a7e8d-109">Se il problema persiste, seguire [questa procedura per](https://aka.ms/pfcte) risolvere i problemi di accesso alle cartelle pubbliche tramite Outlook.</span><span class="sxs-lookup"><span data-stu-id="a7e8d-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="a7e8d-110">**Per controllare quali utenti possono accedere alle cartelle pubbliche tramite Outlook:**</span><span class="sxs-lookup"><span data-stu-id="a7e8d-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="a7e8d-111">Utilizzare Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true o $false</span><span class="sxs-lookup"><span data-stu-id="a7e8d-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="a7e8d-112">$true: consente agli utenti di accedere alle cartelle pubbliche in Outlook</span><span class="sxs-lookup"><span data-stu-id="a7e8d-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="a7e8d-113">$false: consente agli utenti di accedere alle cartelle pubbliche in Outlook. </span><span class="sxs-lookup"><span data-stu-id="a7e8d-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="a7e8d-114">Questo è il valore predefinito.</span><span class="sxs-lookup"><span data-stu-id="a7e8d-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="a7e8d-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="a7e8d-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="a7e8d-116">**Nota** Questa procedura consente di controllare le connessioni solo con il desktop di Outlook per i client Windows.</span><span class="sxs-lookup"><span data-stu-id="a7e8d-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="a7e8d-117">Un utente può continuare ad accedere alle cartelle pubbliche OWA o Outlook per Mac.</span><span class="sxs-lookup"><span data-stu-id="a7e8d-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="a7e8d-118">Per ulteriori informazioni, vedere Annuncio del supporto per le [connessioni controllate alle cartelle pubbliche in Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="a7e8d-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>