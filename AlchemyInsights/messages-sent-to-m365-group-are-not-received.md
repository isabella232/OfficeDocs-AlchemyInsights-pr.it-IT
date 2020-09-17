---
title: I messaggi inviati al gruppo di Microsoft 365 non vengono ricevuti da tutti membri
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d2f0674f6be135927dc5995575c14f3c2708df49
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806151"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="70c5c-102">I messaggi inviati a un gruppo di Microsoft 365 non vengono ricevuti da tutti membri</span><span class="sxs-lookup"><span data-stu-id="70c5c-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="70c5c-103">Assicurarsi che tutti i membri del gruppo abbiano effettuato la sottoscrizione alle e-mail.</span><span class="sxs-lookup"><span data-stu-id="70c5c-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="70c5c-104">Vedere [Seguire un gruppo in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="70c5c-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="70c5c-105">Per controllare lo stato dei messaggi dei membri che hanno effettuato la sottoscrizione alle e-mail del gruppo, eseguire il comando seguente in [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="70c5c-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`