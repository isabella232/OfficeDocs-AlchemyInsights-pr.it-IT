---
title: Utilizzare PowerShell di Exchange Online per abilitare DKIM per un dominio specifico
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500881"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Utilizzare PowerShell di Exchange Online per abilitare DKIM per un dominio specifico

Se non è possibile creare i record DNS DKIM nell'interfaccia di amministrazione, provare a usare PowerShell di Exchange Online. 

Per creare un record DNS DKIM utilizzando PowerShell di Exchange Online, eseguire la procedura seguente:

1. Aprire Windows PowerShell come amministratore ed eseguire i comandi seguenti nella sequenza descritta:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
In caso di problemi durante la connessione a PowerShell di Exchange Online, vedere [Connettersi a PowerShell di Exchange Online.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Dopo aver eseguito la connessione a PowerShell di Exchange Online, eseguire il comando seguente:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Dopo aver eseguito correttamente il comando precedente, eseguire il comando seguente per terminare la sessione di PowerShell di Exchange Online:

    `Remove-PSSession $Session` 



