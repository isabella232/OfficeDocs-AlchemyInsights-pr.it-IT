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
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="b1878-102">I messaggi inviati a un gruppo di Microsoft 365 non vengono ricevuti da tutti membri</span><span class="sxs-lookup"><span data-stu-id="b1878-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="b1878-103">Assicurarsi che tutti i membri del gruppo abbiano effettuato la sottoscrizione alle e-mail.</span><span class="sxs-lookup"><span data-stu-id="b1878-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="b1878-104">Vedere [Seguire un gruppo in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="b1878-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="b1878-105">Per controllare lo stato dei messaggi dei membri che hanno effettuato la sottoscrizione alle e-mail del gruppo, eseguire il comando seguente in [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="b1878-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="b1878-106">Usare il seguente comando EXO di PowerShell per configurare la ricezione dei messaggi di posta elettronica inviati dal gruppo Microsoft 365 a tutti i membri del gruppo:</span><span class="sxs-lookup"><span data-stu-id="b1878-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="b1878-107">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="b1878-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`