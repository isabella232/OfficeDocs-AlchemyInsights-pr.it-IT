---
title: 'Configurare le risposte automatiche per una cassetta postale '
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: aeeb2e1e76fe602d2767b422797452fd1155fdd5
ms.sourcegitcommit: fdfd41c2bfb2d45003b3906e6469377384a91cb5
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2020
ms.locfileid: "43509506"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="9c021-102">Configurare le risposte automatiche per la cassetta postale dell'utente</span><span class="sxs-lookup"><span data-stu-id="9c021-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="9c021-103">**Metodo 1**</span><span class="sxs-lookup"><span data-stu-id="9c021-103">**Method 1**</span></span>

1. <span data-ttu-id="9c021-104">Accedere al portale di Office 365.</span><span class="sxs-lookup"><span data-stu-id="9c021-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="9c021-105">Passare a **Utenti > Utenti attivi** o **Gruppi > Cassette postali condivise** se è stata impostata questa opzione nella cassetta postale condivisa.</span><span class="sxs-lookup"><span data-stu-id="9c021-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="9c021-106">Selezionare un utente con una cassetta postale di Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c021-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="9c021-107">A destra, nel menu a comparsa passare a **Impostazioni di posta > Risposte automatiche**, se si tratta di una cassetta postale condivisa, basta fare clic su **Risposte automatiche** nel riquadro a comparsa.</span><span class="sxs-lookup"><span data-stu-id="9c021-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="9c021-108">**Metodo 2**</span><span class="sxs-lookup"><span data-stu-id="9c021-108">**Method 2**</span></span>

1. <span data-ttu-id="9c021-109">Accedere al portale di amministrazione di Office 365 tramite le credenziali di amministratore.</span><span class="sxs-lookup"><span data-stu-id="9c021-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="9c021-110">Espandere **Interfacce di amministrazione**, poi fare clic su **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="9c021-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="9c021-111">Fare clic sull'immagine nell'angolo in alto a destra, fare clic su **Altro utente** e poi selezionare la cassetta postale utente che si vuole modificare.</span><span class="sxs-lookup"><span data-stu-id="9c021-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="9c021-112">A sinistra, selezionare **Opzioni**, fare clic su **Organizza posta elettronica**e poi fare clic su **Risposte automatiche.**</span><span class="sxs-lookup"><span data-stu-id="9c021-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="9c021-113">**Metodo 3**</span><span class="sxs-lookup"><span data-stu-id="9c021-113">**Method 3**</span></span>

<span data-ttu-id="9c021-114">In PowerShell di Exchange Online, eseguire il cmdlet seguente:</span><span class="sxs-lookup"><span data-stu-id="9c021-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="9c021-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="9c021-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="9c021-116">Per altre informazioni sul cmdlet, vedere [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="9c021-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
