---
title: I messaggi inviati al gruppo di Microsoft 365 non vengono ricevuti da tutti membri
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 29adc5a7b8b74280cb3fcd6369dc4fc3a3e8e957
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823791"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="49fb7-102">I messaggi inviati a un gruppo di Microsoft 365 non vengono ricevuti da tutti membri</span><span class="sxs-lookup"><span data-stu-id="49fb7-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="49fb7-103">Assicurarsi che tutti i membri del gruppo abbiano effettuato la sottoscrizione alle e-mail.</span><span class="sxs-lookup"><span data-stu-id="49fb7-103">Ensure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="49fb7-104">Vedere [Seguire un gruppo in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="49fb7-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="49fb7-105">Per controllare lo stato dei messaggi dei membri che hanno effettuato la sottoscrizione alle e-mail del gruppo, eseguire il comando seguente in [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="49fb7-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="49fb7-106">Usare il seguente comando EXO di PowerShell per configurare la ricezione dei messaggi di posta elettronica inviati dal gruppo Microsoft 365 a tutti i membri del gruppo:</span><span class="sxs-lookup"><span data-stu-id="49fb7-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="49fb7-107">Ad esempio:</span><span class="sxs-lookup"><span data-stu-id="49fb7-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`