---
title: Livelli di autorizzazione di SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760697"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="e14bb-102">Problemi di connessione di SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="e14bb-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="e14bb-103">Se in SharePoint Designer si verificano problemi di connessione per i siti di SharePoint, provare a eseguire le soluzioni comuni seguenti.</span><span class="sxs-lookup"><span data-stu-id="e14bb-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="e14bb-104">Passaggio 1: verificare che SharePoint Designer sia stato aggiornato.</span><span class="sxs-lookup"><span data-stu-id="e14bb-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="e14bb-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="e14bb-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="e14bb-106">SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="e14bb-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="e14bb-107">Aggiornamento per SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="e14bb-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="e14bb-108">Passaggio 2: cancellare i file della cache locale</span><span class="sxs-lookup"><span data-stu-id="e14bb-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="e14bb-109">Chiudere SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="e14bb-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="e14bb-110">Nel computer locale, passare alla cartella seguente per rimuovere i file memorizzati nella cache.</span><span class="sxs-lookup"><span data-stu-id="e14bb-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="e14bb-111">Fare clic sul pulsante Start, scegliere Esegui ed eliminare tutti i file trovati in ognuna delle posizioni seguenti.</span><span class="sxs-lookup"><span data-stu-id="e14bb-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="e14bb-112">%APPDATA%\Microsoft\Web server Extensions\Cache%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="e14bb-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="e14bb-113">Aprire SharePoint Designer 2013 e immettere di nuovo l'account per verificare se funziona.</span><span class="sxs-lookup"><span data-stu-id="e14bb-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="e14bb-114">Passaggio 3: [abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="e14bb-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="e14bb-115">Passaggio 4: è necessario che gli amministratori consentano lo script personalizzato per consentire la connessione di SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="e14bb-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="e14bb-116">Per la procedura dettagliata, esempi e considerazioni, vedere [Allow or impedisce script personalizzato](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="e14bb-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


