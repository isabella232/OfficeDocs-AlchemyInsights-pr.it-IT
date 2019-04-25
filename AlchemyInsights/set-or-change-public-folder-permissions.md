---
title: Impostare o modificare le autorizzazioni per le cartelle pubbliche
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: d1554e8a63455f3549044e526183c0e8709f2631
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/23/2019
ms.locfileid: "32421820"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="e3004-102">Autorizzazioni e cartelle pubbliche</span><span class="sxs-lookup"><span data-stu-id="e3004-102">Permissions and Public Folders</span></span>

<span data-ttu-id="e3004-103">È possibile modificare le autorizzazioni per le cartelle pubbliche utilizzando Outlook, l'interfaccia di amministrazione di Exchange (EAC) o PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e3004-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="e3004-104">Per le istruzioni di Outlook, [fare clic qui](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="e3004-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="e3004-105">Per l'interfaccia di amministrazione di Exchange, fare riferimento a [questo articolo](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) per istruzioni.</span><span class="sxs-lookup"><span data-stu-id="e3004-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> <span data-ttu-id="e3004-106">È possibile fare clic [qui](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) per accedere a EAC.</span><span class="sxs-lookup"><span data-stu-id="e3004-106">You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="e3004-107">Per PowerShell, fare riferimento a [questo articolo](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) per istruzioni sull'utilizzo del cmdlet sharepointsync Add-PublicFolderClientPermission.</span><span class="sxs-lookup"><span data-stu-id="e3004-107">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="e3004-108">Se sono necessarie istruzioni per la connessione a Exchange PowerShell, fare clic [qui](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="e3004-108">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="e3004-109">Se **gli utenti esterni non possono inviare posta elettronica a una cartella pubblica abilitata alla posta elettronica**, il motivo potrebbe essere che la cartella pubblica non disponga delle autorizzazioni necessarie per il recapito esterno della posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="e3004-109">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="e3004-110">È possibile risolvere questo argomento utilizzando le istruzioni di Outlook [qui](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)o le istruzioni di PowerShell [qui](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="e3004-110">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

