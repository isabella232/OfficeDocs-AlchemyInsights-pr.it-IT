---
title: Accedere a Windows 10 senza usare una password
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830550"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="a8e53-102">Accedere a Windows 10 senza usare una password</span><span class="sxs-lookup"><span data-stu-id="a8e53-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="a8e53-103">Per evitare di dover digitare una password all'avvio di Windows, ti consigliamo di usare una delle opzioni di accesso sicuro di Windows Hello, ad esempio un PIN, un riconoscimento facciale o un'impronta digitale, se disponibile.</span><span class="sxs-lookup"><span data-stu-id="a8e53-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="a8e53-104">Se vuoi veramente disabilitare l'accesso sicuro, vedi le istruzioni "Accedi automaticamente a Windows 10" di seguito.</span><span class="sxs-lookup"><span data-stu-id="a8e53-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="a8e53-105">**Proteggere le alternative di Windows Hello alla password dell'account**</span><span class="sxs-lookup"><span data-stu-id="a8e53-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="a8e53-106">Vai a **Impostazioni > account > opzioni di** accesso (o fai clic [qui](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="a8e53-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="a8e53-107">Verranno elencate le opzioni di accesso disponibili.</span><span class="sxs-lookup"><span data-stu-id="a8e53-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="a8e53-108">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="a8e53-108">For example:</span></span>

![Opzioni di accesso.](media/sign-in-options.png)

<span data-ttu-id="a8e53-110">Tocca o fai clic su una delle opzioni per configurarlo.</span><span class="sxs-lookup"><span data-stu-id="a8e53-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="a8e53-111">Al successivo avvio o sblocco di Windows, potrai usare la nuova opzione anziché una password.</span><span class="sxs-lookup"><span data-stu-id="a8e53-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="a8e53-112">**Accedi automaticamente a Windows 10**</span><span class="sxs-lookup"><span data-stu-id="a8e53-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="a8e53-113">**Nota:** l'accesso automatico è pratico, ma introduce un rischio per la sicurezza, soprattutto se il PC è accessibile da più persone.</span><span class="sxs-lookup"><span data-stu-id="a8e53-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="a8e53-114">Tocca o fai clic sul **pulsante Start** nella barra delle applicazioni.</span><span class="sxs-lookup"><span data-stu-id="a8e53-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="a8e53-115">Digitare **netplwiz** e premere INVIO per aprire la finestra Account utente.</span><span class="sxs-lookup"><span data-stu-id="a8e53-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="a8e53-116">In **Account utente** fare clic sull'account a cui si desidera accedere automaticamente all'avvio di Windows.</span><span class="sxs-lookup"><span data-stu-id="a8e53-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="a8e53-117">Deseleziona la casella di controllo "Gli utenti devono immettere un nome utente e una password per usare questo computer".</span><span class="sxs-lookup"><span data-stu-id="a8e53-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Gli utenti devono immettere un nome utente e una password.](media/users-must-enter-username.png)

5. <span data-ttu-id="a8e53-119">Fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="a8e53-119">Click **OK**.</span></span> <span data-ttu-id="a8e53-120">Verrà richiesto di immettere e confermare la password per l'account selezionato.</span><span class="sxs-lookup"><span data-stu-id="a8e53-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="a8e53-121">Fare clic su **OK** per terminare.</span><span class="sxs-lookup"><span data-stu-id="a8e53-121">Click **OK** to finish.</span></span> <span data-ttu-id="a8e53-122">Al successivo avvio di Windows 10, accederà automaticamente all'account selezionato.</span><span class="sxs-lookup"><span data-stu-id="a8e53-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
