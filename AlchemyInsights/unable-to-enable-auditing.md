---
title: 2419-Impossibile-attivare-controllo
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510432"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="726ac-102">Impossibile abilitare il controllo unificato</span><span class="sxs-lookup"><span data-stu-id="726ac-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="726ac-103">Quando si tenta di abilitare il controllo unificato per l'organizzazione, è possibile che venga visualizzato un errore simile al seguente:</span><span class="sxs-lookup"><span data-stu-id="726ac-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="726ac-104">Per risolvere il problema, attenersi alla seguente procedura:</span><span class="sxs-lookup"><span data-stu-id="726ac-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="726ac-105">[Connettersi a PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="726ac-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="726ac-106">Eseguire il seguente cmdlet:</span><span class="sxs-lookup"><span data-stu-id="726ac-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="726ac-107">Attendere 60 minuti per rendere effettive le impostazioni precedenti.</span><span class="sxs-lookup"><span data-stu-id="726ac-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="726ac-108">Eseguire il seguente comando in PowerShell di Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="726ac-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="726ac-109">Per ulteriori informazioni, vedere gli articoli seguenti:</span><span class="sxs-lookup"><span data-stu-id="726ac-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="726ac-110">Connettersi a PowerShell di Exchange Online utilizzando l'autenticazione a più fattori</span><span class="sxs-lookup"><span data-stu-id="726ac-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="726ac-111">Abilitare o disabilitare la ricerca nel log di controllo</span><span class="sxs-lookup"><span data-stu-id="726ac-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
