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
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320360"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Impostare ClientAccessServerEnabled su True

Se non è possibile aprire un messaggio di posta elettronica crittografato e visualizzare invece un allegato **rpmsg,** eseguire la procedura seguente:

1. Connettersi a PowerShell di Exchange Online.

    **Nota:** per connettersi a Exchange Online PowerShell, è necessario accedere utilizzando un account amministratore globale o Exchange amministratore.

   a. Aprire Windows PowerShell ed eseguire il comando seguente:`$UserCredential = Get-Credential`
   b. Nella finestra **Windows PowerShell richiesta credenziali** immettere l'account aziendale o dell'istituto di istruzione e la password, c. Fare clic su **OK**. 

2. Eseguire il comando seguente per creare una nuova sessione:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Eseguire il comando riportato di seguito:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Eseguire `Get-IRMConfiguration` il comando.

4. Controllare **l'impostazione ClientAccessServerEnabled.** 

    a. Se **l'impostazione ClientAccessServerEnabled** è impostata su **False,** eseguire il cmdlet seguente: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Suggerimento:** chiudi sempre la sessione powershell con il comando seguente: `Remove-PSSession $Session`

Per ulteriori informazioni, vedere [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

