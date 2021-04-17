---
title: 'Configurare le risposte automatiche per una cassetta postale '
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820938"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="5b9c0-102">Configurare le risposte automatiche per la cassetta postale dell'utente</span><span class="sxs-lookup"><span data-stu-id="5b9c0-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="5b9c0-103">**Metodo 1**</span><span class="sxs-lookup"><span data-stu-id="5b9c0-103">**Method 1**</span></span>

1. <span data-ttu-id="5b9c0-104">Accedere al portale di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5b9c0-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="5b9c0-105">Passare a **Utenti > Utenti attivi** o **Gruppi > Cassette postali condivise** se è stata impostata questa opzione nella cassetta postale condivisa.</span><span class="sxs-lookup"><span data-stu-id="5b9c0-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="5b9c0-106">Selezionare un utente con una cassetta postale di Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b9c0-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="5b9c0-107">A destra, nel menu a comparsa passare a **Impostazioni di posta > Risposte automatiche**, se si tratta di una cassetta postale condivisa, basta fare clic su **Risposte automatiche** nel riquadro a comparsa.</span><span class="sxs-lookup"><span data-stu-id="5b9c0-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="5b9c0-108">**Metodo 2**</span><span class="sxs-lookup"><span data-stu-id="5b9c0-108">**Method 2**</span></span>

1. <span data-ttu-id="5b9c0-109">Accedere al portale di amministrazione di Microsoft 365 tramite le credenziali di amministratore.</span><span class="sxs-lookup"><span data-stu-id="5b9c0-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="5b9c0-110">Espandere **Interfacce di amministrazione**, poi fare clic su **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="5b9c0-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="5b9c0-111">Fare clic sull'immagine nell'angolo in alto a destra, fare clic su **Altro utente** e poi selezionare la cassetta postale utente che si vuole modificare.</span><span class="sxs-lookup"><span data-stu-id="5b9c0-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="5b9c0-112">A sinistra, selezionare **Opzioni**, fare clic su **Organizza posta elettronica** e poi fare clic su **Risposte automatiche.**</span><span class="sxs-lookup"><span data-stu-id="5b9c0-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="5b9c0-113">**Metodo 3**</span><span class="sxs-lookup"><span data-stu-id="5b9c0-113">**Method 3**</span></span>

<span data-ttu-id="5b9c0-114">In PowerShell di Exchange Online, eseguire il cmdlet seguente:</span><span class="sxs-lookup"><span data-stu-id="5b9c0-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="5b9c0-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="5b9c0-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="5b9c0-116">Per altre informazioni sul cmdlet, vedere [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="5b9c0-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
