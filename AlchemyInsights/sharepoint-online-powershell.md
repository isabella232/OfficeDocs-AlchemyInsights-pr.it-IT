---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709074"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Utilizzare PowerShell o script all'interno di Sharepoint Online? Per ulteriori informazioni, visitare i collegamenti seguenti.
- [Guida introduttiva a SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Connettersi a PowerShell di SpO con l'autenticazione a più fattori (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contiene una raccolta di comandi di PowerShell che consente di eseguire azioni di gestione complesse per SharePoint SharePoint.

> [!NOTE]
> - Se si verificano problemi di connessione con SpO Management Shell, assicurarsi di aver aggiornato la versione più recente e provare a [reimportare](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) il modulo utilizzando *"Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Se si sta tentando di eseguire script del modello a oggetti sul lato client, è necessario che [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) sia installato nel computer locale.
> - Se si verificano problemi durante l'esecuzione di script da PowerShell, è consigliabile eseguire PowerShell come amministratore e modificare i [criteri di esecuzione.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)