---
title: PowerShell di SharePoint Online
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123003"
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