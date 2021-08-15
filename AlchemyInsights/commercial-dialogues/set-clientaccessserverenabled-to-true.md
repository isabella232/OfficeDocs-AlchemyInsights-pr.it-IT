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
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994869"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Impostare ClientAccessServerEnabled su True

Se non è possibile aprire un messaggio di posta elettronica crittografato e visualizzare invece un allegato **rpmsg,** eseguire la procedura seguente:

1. Connettersi a PowerShell di Exchange Online.

> [!NOTE]
> Per connettersi a Exchange Online PowerShell, è necessario accedere utilizzando un account amministratore globale o Exchange amministratore.

   a. Aprire Windows PowerShell ed eseguire il comando seguente:`$UserCredential = Get-Credential`
b. Nella finestra **Windows PowerShell richiesta credenziali** immettere l'account aziendale o dell'istituto di istruzione e la password, c. Fare clic su **OK**. 

2. Eseguire il comando seguente per creare una nuova sessione:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Eseguire il comando seguente:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Eseguire `Get-IRMConfiguration` il comando.

4. Controllare **l'impostazione ClientAccessServerEnabled.** 

    a. Se **l'impostazione ClientAccessServerEnabled** è impostata su **False,** eseguire il cmdlet seguente: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Chiudi sempre la sessione di PowerShell con il comando seguente: `Remove-PSSession $Session`

Per ulteriori informazioni, vedere [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

