---
title: Accedere a Windows 10 senza utilizzare una password
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719957"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="33c24-102">Accedere a Windows 10 senza utilizzare una password</span><span class="sxs-lookup"><span data-stu-id="33c24-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="33c24-103">Per evitare di dover digitare una password all'avvio di Windows, si consiglia di utilizzare una delle opzioni di accesso sicuro di Windows Hello, come un PIN, il riconoscimento del volto o l'impronta digitale, se disponibile.</span><span class="sxs-lookup"><span data-stu-id="33c24-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="33c24-104">Se si vuole davvero disabilitare l'accesso sicuro, vedere le istruzioni "Accedi automaticamente a Windows 10" di seguito.</span><span class="sxs-lookup"><span data-stu-id="33c24-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="33c24-105">**Protezione delle alternative di Windows Hello per la password dell'account**</span><span class="sxs-lookup"><span data-stu-id="33c24-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="33c24-106">Andare a **impostazioni > account > opzioni di accesso** (o fare clic [qui](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="33c24-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="33c24-107">Vengono elencate le opzioni di accesso disponibili.</span><span class="sxs-lookup"><span data-stu-id="33c24-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="33c24-108">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="33c24-108">For example:</span></span>

![Opzioni di accesso.](media/sign-in-options.png)

<span data-ttu-id="33c24-110">Fare clic o toccare una delle opzioni per configurarla.</span><span class="sxs-lookup"><span data-stu-id="33c24-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="33c24-111">La volta successiva che si avvia o si sblocca Windows, è possibile utilizzare la nuova opzione invece di una password.</span><span class="sxs-lookup"><span data-stu-id="33c24-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="33c24-112">**Accesso automatico a Windows 10**</span><span class="sxs-lookup"><span data-stu-id="33c24-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="33c24-113">**Nota**: l'accesso automatico è comodo, ma introduce un rischio per la sicurezza, soprattutto se il PC è accessibile da più persone.</span><span class="sxs-lookup"><span data-stu-id="33c24-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="33c24-114">Fare clic o toccare il pulsante **Start** nella barra delle applicazioni.</span><span class="sxs-lookup"><span data-stu-id="33c24-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="33c24-115">Digitare **Netplwiz** e premere INVIO per aprire la finestra account utente.</span><span class="sxs-lookup"><span data-stu-id="33c24-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="33c24-116">In **account utente**, fare clic sull'account che si desidera accedere automaticamente al momento dell'avvio di Windows.</span><span class="sxs-lookup"><span data-stu-id="33c24-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="33c24-117">Deselezionare la casella di controllo "gli utenti devono immettere un nome utente e una password per l'utilizzo del computer".</span><span class="sxs-lookup"><span data-stu-id="33c24-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Gli utenti devono immettere l'opzione nome utente e password.](media/users-must-enter-username.png)

5. <span data-ttu-id="33c24-119">Fare clic su **OK**.</span><span class="sxs-lookup"><span data-stu-id="33c24-119">Click **OK**.</span></span> <span data-ttu-id="33c24-120">Verrà chiesto di immettere e confermare la password per l'account selezionato.</span><span class="sxs-lookup"><span data-stu-id="33c24-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="33c24-121">Fare clic su **OK** per terminare.</span><span class="sxs-lookup"><span data-stu-id="33c24-121">Click **OK** to finish.</span></span> <span data-ttu-id="33c24-122">La volta successiva che viene avviato Windows 10, l'utente accede automaticamente all'account selezionato.</span><span class="sxs-lookup"><span data-stu-id="33c24-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
