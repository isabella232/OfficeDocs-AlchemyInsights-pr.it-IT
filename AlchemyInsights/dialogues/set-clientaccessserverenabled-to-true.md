---
title: Impostare ClientAccessServerEnabled su True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509746"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Impostare ClientAccessServerEnabled su True

Se non è possibile aprire un messaggio di posta elettronica crittografato e viene invece visualizzato un allegato **rpmsg,** eseguire la procedura seguente:

1. Connettersi a PowerShell di Exchange Online.

> [!NOTE]
> Per connettersi a PowerShell di Exchange Online, è necessario accedere utilizzando un account di amministratore globale o di amministratore di Exchange.

   a. Aprire Windows PowerShell ed eseguire il comando seguente: `$UserCredential = Get-Credential`
b. Nella finestra **Windows PowerShell richiesta** credenziali immettere l'account aziendale o dell'istituto di istruzione e la password, c. Fare clic su **OK**. 

2. Eseguire il comando seguente per creare una nuova sessione:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Eseguire il comando seguente:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Esegui `Get-IRMConfiguration` il comando.

4. Controllare **l'impostazione ClientAccessServerEnabled.** 

    a. Se **l'impostazione ClientAccessServerEnabled** è impostata su **False,** eseguire il cmdlet seguente: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Chiudere sempre la sessione di PowerShell con il comando seguente: `Remove-PSSession $Session`

Per ulteriori informazioni, vedere [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

