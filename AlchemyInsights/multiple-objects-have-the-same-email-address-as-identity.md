---
title: Più oggetti hanno lo stesso indirizzo di posta elettronica come identità
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431537"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="b627a-102">Più oggetti hanno lo stesso indirizzo di posta elettronica come identità</span><span class="sxs-lookup"><span data-stu-id="b627a-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="b627a-103">**Più oggetti**</span><span class="sxs-lookup"><span data-stu-id="b627a-103">**Multiple objects**</span></span>

<span data-ttu-id="b627a-104">Una delle cause più comuni di questo errore consiste nell’impossibilità di instradare correttamente una richiesta di Outlook Web App in presenza di più oggetti con lo stesso indirizzo di posta elettronica come identità.</span><span class="sxs-lookup"><span data-stu-id="b627a-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="b627a-105">Per trovare tali oggetti, eseguire i comandi seguenti:</span><span class="sxs-lookup"><span data-stu-id="b627a-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="b627a-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="b627a-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="b627a-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="b627a-107">· Get-User <email address></span></span>

<span data-ttu-id="b627a-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="b627a-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="b627a-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="b627a-109">· Get-Contact <email address></span></span>

<span data-ttu-id="b627a-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="b627a-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="b627a-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="b627a-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="b627a-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="b627a-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="b627a-113">Per risolvere il problema, rimuovere gli oggetti con la stessa identità di posta elettronica e verificare che sia presente un singolo oggetto con una identità di posta elettronica specifica e che il relativo tipo di destinatario sia UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="b627a-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="b627a-114">**Lo stesso indirizzo viene usato per le cassette postali aziendali e degli utenti privati**</span><span class="sxs-lookup"><span data-stu-id="b627a-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="b627a-115">Un’altra causa consiste nell’usare lo stesso indirizzo per le cassette postali aziendali e degli utenti privati.</span><span class="sxs-lookup"><span data-stu-id="b627a-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="b627a-116">In questo caso, è necessario che l'utente modifichi il suo alias consumer principale finché Cafe non supporta questo scenario.</span><span class="sxs-lookup"><span data-stu-id="b627a-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="b627a-117">Si tratta di un errore permanente che non scompare senza un intervento.</span><span class="sxs-lookup"><span data-stu-id="b627a-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="b627a-118">Per informazioni dettagliate, vedere [Cambiare l'indirizzo di posta elettronica o il numero di telefono per l’account Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="b627a-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>