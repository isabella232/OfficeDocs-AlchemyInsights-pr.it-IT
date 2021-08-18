---
title: Invia come gruppo Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086132"
---
# <a name="send-as-microsoft-365-group"></a>Invia come gruppo Microsoft 365

È possibile assegnare autorizzazioni Invia come per consentire a utenti specifici di inviare messaggi come gruppo di Microsoft 365:  

1. Connettersi a PowerShell di Exchange Online.  

2. Eseguire il comando seguente:  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

Per maggiori informazioni, vedere [Consentire ai membri di inviare un messaggio da o per conto di un gruppo](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).