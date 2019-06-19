---
title: 2419-Impossibile-attivare-controllo
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065661"
---
# <a name="unable-to-enable-unified-auditing"></a>Impossibile abilitare il controllo unificato

Quando si tenta di abilitare il controllo unificato per l'organizzazione di Office 365, è possibile che venga visualizzato un errore simile al seguente:

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

-  [Abilitare o disabilitare la ricerca nel log di controllo di Office 365](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
