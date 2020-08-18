---
title: PowerShell di SharePoint Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786893"
---
# <a name="sharepoint-online-powershell"></a>PowerShell di SharePoint Online

Utilizzo di PowerShell o script all'interno di SharePoint Online Per ulteriori informazioni, visitare i collegamenti riportati di seguito.
- [Guida introduttiva a SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Connettersi a SPO PowerShell con autenticazione a più fattori (AMF)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- I [modelli e le procedure di SharePoint (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contengono una raccolta di comandi di PowerShell che consente di eseguire azioni di gestione complesse verso spo.

> [!NOTE]
> - Se si verificano problemi di connessione con la shell di gestione di SPO, accertarsi di aver aggiornato la versione più recente e provare a [reimportare il modulo](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) utilizzando *"Import-Module Microsoft. online. SharePoint. PowerShell".*
> - Se si sta tentando di eseguire script del modello a oggetti sul fianco client, è necessario che l' [SDK dei componenti client di SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) sia installato nel computer locale.
> - Se si verificano problemi con gli script di PowerShell, è possibile prendere in considerazione l'esecuzione di PowerShell come amministratore e la modifica dei [criteri di esecuzione](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).