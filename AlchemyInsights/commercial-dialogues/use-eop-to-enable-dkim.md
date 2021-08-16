---
title: Utilizzare Exchange Online PowerShell per abilitare DKIM per un dominio specifico
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070308"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Utilizzare Exchange Online PowerShell per abilitare DKIM per un dominio specifico

Se non è possibile creare i record DNS DKIM nell'interfaccia di amministrazione, provare a usare Exchange Online PowerShell. 

Per creare un record DNS DKIM Exchange Online PowerShell, eseguire la procedura seguente:

1. Aprire Windows PowerShell amministratore ed eseguire i comandi seguenti nella sequenza descritta:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
In caso di problemi di connessione a Exchange Online PowerShell, [vedere Connessione a Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Dopo aver eseguito la connessione a Exchange Online PowerShell, eseguire il comando seguente:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Dopo aver eseguito correttamente il comando precedente, eseguire il comando seguente per terminare la sessione Exchange Online PowerShell:

    `Remove-PSSession $Session` 



