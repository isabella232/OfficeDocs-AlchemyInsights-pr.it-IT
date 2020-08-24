---
title: Invia come gruppo Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/21/2020
ms.locfileid: "46853005"
---
# <a name="send-as-microsoft-365-group"></a>Invia come gruppo Microsoft 365

È possibile assegnare autorizzazioni Invia come per consentire a utenti specifici di inviare messaggi come gruppo di Microsoft 365:  

1. Connettersi a PowerShell di Exchange Online.  

2. Eseguire il comando seguente:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Per maggiori informazioni, vedere [Consentire ai membri di inviare un messaggio da o per conto di un gruppo](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).