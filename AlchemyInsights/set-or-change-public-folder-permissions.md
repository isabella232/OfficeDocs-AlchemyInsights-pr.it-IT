---
title: Impostare o modificare le autorizzazioni per le cartelle pubbliche
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
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e419c72a890e68fc7b6d40d2b64406e42f9b0769
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51789211"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="d6fd3-102">Autorizzazioni e cartelle pubbliche</span><span class="sxs-lookup"><span data-stu-id="d6fd3-102">Permissions and Public Folders</span></span>

<span data-ttu-id="d6fd3-103">È possibile modificare le autorizzazioni per le cartelle pubbliche utilizzando Outlook, l'interfaccia di amministrazione di Exchange (EAC) o PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d6fd3-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="d6fd3-104">Per le istruzioni di Outlook, [fare clic qui](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="d6fd3-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="d6fd3-105">Per EAC, fare riferimento [a questo articolo per](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) istruzioni.</span><span class="sxs-lookup"><span data-stu-id="d6fd3-105">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions.</span></span> 
    
- <span data-ttu-id="d6fd3-106">Per PowerShell, fare riferimento [a questo articolo](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) per istruzioni sull'uso del Add-PublicFolderClientPermission comando.</span><span class="sxs-lookup"><span data-stu-id="d6fd3-106">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet.</span></span> <span data-ttu-id="d6fd3-107">Se sono necessarie istruzioni per connettersi a PowerShell di Exchange, fare clic [qui](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="d6fd3-107">If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="d6fd3-108">Se **gli utenti esterni non possono** inviare messaggi di posta elettronica a una cartella pubblica abilitata alla posta elettronica, il motivo potrebbe essere che la cartella pubblica non dispone delle autorizzazioni necessarie per il recapito esterno della posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="d6fd3-108">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery.</span></span> <span data-ttu-id="d6fd3-109">È possibile risolvere il problema usando le istruzioni di Outlook [qui](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)o le istruzioni di PowerShell [qui](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="d6fd3-109">You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  

