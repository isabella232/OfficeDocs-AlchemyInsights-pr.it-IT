---
title: I messaggi inviati al gruppo di Microsoft 365 non vengono ricevuti da tutti membri
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d222eb92d806bad52264139a8ddba72f323b3783
ms.sourcegitcommit: 10cfd9d552b0d8a096bcef34e82c04a4c166a13a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50479457"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>I messaggi inviati a un gruppo di Microsoft 365 non vengono ricevuti da tutti membri

Assicurarsi che tutti i membri del gruppo abbiano effettuato la sottoscrizione alle e-mail. Vedere [Seguire un gruppo in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Per controllare lo stato dei messaggi dei membri che hanno effettuato la sottoscrizione alle e-mail del gruppo, eseguire il comando seguente in [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Usare il seguente comando EXO di PowerShell per configurare la ricezione dei messaggi di posta elettronica inviati dal gruppo Microsoft 365 a tutti i membri del gruppo:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Ad esempio:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`