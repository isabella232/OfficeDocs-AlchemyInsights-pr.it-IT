---
title: Problemi di connessione di SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508427"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="e6873-102">Problemi di connessione di SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="e6873-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="e6873-103">Se in SharePoint Designer si verificano problemi di connessione per i siti di SharePoint, provare a eseguire le soluzioni comuni seguenti.</span><span class="sxs-lookup"><span data-stu-id="e6873-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="e6873-104">Passaggio 1: verificare che SharePoint Designer 2013 sia stato aggiornato con [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e l' [aggiornamento del 2 agosto 2016 per SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="e6873-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="e6873-105">Passaggio 2: cancellare i file della cache locale:</span><span class="sxs-lookup"><span data-stu-id="e6873-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="e6873-106">Chiudere SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="e6873-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="e6873-107">Nel computer locale, rimuovere tutti i file trovati in ognuna delle cartelle seguenti.</span><span class="sxs-lookup"><span data-stu-id="e6873-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="e6873-108">Extensions\Cache del server%APPDATA%\Microsoft\Web</span><span class="sxs-lookup"><span data-stu-id="e6873-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="e6873-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="e6873-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="e6873-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="e6873-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="e6873-111">Aprire SharePoint Designer 2013 e immettere di nuovo l'account per verificare se funziona.</span><span class="sxs-lookup"><span data-stu-id="e6873-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="e6873-112">Passaggio 3: [abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="e6873-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="e6873-113">Passaggio 4: gli amministratori dovranno **consentire lo script personalizzato** nelle impostazioni dell'interfaccia di amministrazione di SharePoint per consentire la connessione a SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="e6873-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="e6873-114">Per ulteriori informazioni, vedere [Consenti o Impedisci lo script personalizzato](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="e6873-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


