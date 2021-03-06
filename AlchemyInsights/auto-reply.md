---
title: 'Per configurare la risposta automatica per tutti i messaggi di posta elettronica inviati al gruppo di Microsoft 365:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: c3c1d4e6b16b54d92771d7bdecdc9cb12bbf888c
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430738"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a><span data-ttu-id="788c0-102">Per configurare la risposta automatica per tutti i messaggi di posta elettronica inviati al gruppo di Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="788c0-102">To configure auto reply for all emails sent to Microsoft 365 group:</span></span>

<span data-ttu-id="788c0-103">**Connettersi a ExO PowerShell usando l'account di amministratore del tenant e usare il comando**:</span><span class="sxs-lookup"><span data-stu-id="788c0-103">**Connect to EXO PowerShell using tenant admin account and use following command**:</span></span>

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> <span data-ttu-id="788c0-104">Sostituire **groupmailbox** con il nome del gruppo su cui si vuole configurare la risposta automatica.</span><span class="sxs-lookup"><span data-stu-id="788c0-104">Change **groupmailbox** to a group name that you want to configure auto reply on.</span></span>

