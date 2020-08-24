---
title: Il mittente non riceve la posta elettronica inviata al gruppo Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/21/2020
ms.locfileid: "46846057"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Il mittente non riceve la posta elettronica inviata al gruppo Microsoft 365

Per impostazione predefinita, il mittente di un messaggio di posta elettronica a un gruppo di Microsoft 365 non riceve una copia del messaggio nella propria posta in arrivo, anche se il mittente è un membro del gruppo.

Usare il comando EXO PowerShell per consentire al mittente di ricevere una copia di ogni messaggio inviato al gruppo Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Per abilitare l'opzione per tutte le cassette postali contemporaneamente:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Nota** Le modifiche apportate a questa impostazione richiedono fino a un’ora per diventare effettive.