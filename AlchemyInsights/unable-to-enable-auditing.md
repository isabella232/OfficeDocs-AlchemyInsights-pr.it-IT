---
title: 2419-Impossibile-attivare-controllo
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767603"
---
# <a name="unable-to-enable-unified-auditing"></a>Impossibile abilitare il controllo unificato

Quando si tenta di abilitare il controllo unificato per l'organizzazione, è possibile che venga visualizzato un errore simile al seguente:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Per risolvere il problema, attenersi alla seguente procedura:

1. [Connettersi a PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Eseguire il seguente cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Attendere 60 minuti per rendere effettive le impostazioni precedenti.

4. Eseguire il seguente comando in PowerShell di Exchange Online:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Per ulteriori informazioni, vedere gli articoli seguenti:

- [Connettersi a PowerShell di Exchange Online utilizzando l'autenticazione a più fattori](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Abilitare o disabilitare la ricerca nel log di controllo](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
