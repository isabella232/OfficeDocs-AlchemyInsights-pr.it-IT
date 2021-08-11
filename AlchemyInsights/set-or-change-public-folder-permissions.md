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
ms.openlocfilehash: 1868b8b04df012d44781f86ee75120ca443af5be5801074329f17c0e40a5acc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060896"
---
# <a name="permissions-and-public-folders"></a>Autorizzazioni e cartelle pubbliche

È possibile modificare le autorizzazioni per le cartelle pubbliche usando Outlook, l'interfaccia di amministrazione di Exchange (EAC) o PowerShell:
  
- Per Outlook istruzioni, [fare clic qui.](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx)
    
- Per EAC, fare riferimento [a questo articolo per](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) istruzioni. 
    
- Per PowerShell, fare riferimento [a questo articolo](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) per istruzioni sull'uso del Add-PublicFolderClientPermission comando. Se sono necessarie istruzioni per connettersi a Exchange PowerShell, fare clic [qui](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).
    
Se **gli utenti esterni non possono** inviare messaggi di posta elettronica a una cartella pubblica abilitata alla posta elettronica, il motivo potrebbe essere che la cartella pubblica non dispone delle autorizzazioni necessarie per il recapito esterno della posta elettronica. Puoi risolvere il problema usando le istruzioni Outlook [qui](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1)o le istruzioni di PowerShell [qui](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).
  

