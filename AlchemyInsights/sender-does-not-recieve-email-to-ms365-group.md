---
title: Il mittente non riceve la posta elettronica inviata al gruppo Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958301"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Il mittente non riceve la posta elettronica inviata al gruppo Microsoft 365

Per impostazione predefinita, il mittente di un messaggio di posta elettronica a un gruppo di Microsoft 365 non riceve una copia del messaggio nella propria posta in arrivo, anche se il mittente è un membro del gruppo.

Usare il comando EXO PowerShell per consentire al mittente di ricevere una copia di ogni messaggio inviato al gruppo Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Per abilitare l'opzione per tutte le cassette postali contemporaneamente:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Nota** Le modifiche apportate a questa impostazione richiedono fino a un’ora per diventare effettive.