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
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="3bd68-102">PowerShell di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="3bd68-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="3bd68-103">Utilizzo di PowerShell o script all'interno di SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="3bd68-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="3bd68-104">Per ulteriori informazioni, visitare i collegamenti riportati di seguito.</span><span class="sxs-lookup"><span data-stu-id="3bd68-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="3bd68-105">Guida introduttiva a SharePoint Online Management Shell</span><span class="sxs-lookup"><span data-stu-id="3bd68-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="3bd68-106">Connettersi a SPO PowerShell con autenticazione a più fattori (AMF)</span><span class="sxs-lookup"><span data-stu-id="3bd68-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="3bd68-107">I [modelli e le procedure di SharePoint (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contengono una raccolta di comandi di PowerShell che consente di eseguire azioni di gestione complesse verso spo.</span><span class="sxs-lookup"><span data-stu-id="3bd68-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="3bd68-108">Se si verificano problemi di connessione con la shell di gestione di SPO, accertarsi di aver aggiornato la versione più recente e provare a [reimportare il modulo](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) utilizzando *"Import-Module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="3bd68-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="3bd68-109">Se si sta tentando di eseguire script del modello a oggetti sul fianco client, è necessario che l' [SDK dei componenti client di SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) sia installato nel computer locale.</span><span class="sxs-lookup"><span data-stu-id="3bd68-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="3bd68-110">Se si verificano problemi con gli script di PowerShell, è possibile prendere in considerazione l'esecuzione di PowerShell come amministratore e la modifica dei [criteri di esecuzione](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="3bd68-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>