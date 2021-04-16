---
title: Abilitare il controllo delle cassette postali
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: c04f27edc1e22e0e4269758827d5468767967be8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814196"
---
# <a name="enable-mailbox-auditing"></a>Abilitare il controllo delle cassette postali

Per abilitare il controllo delle cassette postali per un singolo utente o un'intera organizzazione, è necessario eseguire i cmdlet seguenti da Remote Power Shell:
  
 **Singolo utente**
  
Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
  
 **Organizzazione**
  
Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true
  
[Altre informazioni](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

