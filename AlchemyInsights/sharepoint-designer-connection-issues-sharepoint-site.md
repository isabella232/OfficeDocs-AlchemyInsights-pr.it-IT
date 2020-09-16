---
title: Problemi di connessione di SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727175"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="cea3d-102">Problemi di connessione di SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="cea3d-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="cea3d-103">Se in SharePoint Designer si verificano problemi di connessione per i siti di SharePoint, provare a eseguire le soluzioni comuni seguenti.</span><span class="sxs-lookup"><span data-stu-id="cea3d-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="cea3d-104">Passaggio 1: verificare che SharePoint Designer 2013 sia stato aggiornato con [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) e l' [aggiornamento del 2 agosto 2016 per SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="cea3d-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="cea3d-105">Passaggio 2: cancellare i file della cache locale:</span><span class="sxs-lookup"><span data-stu-id="cea3d-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="cea3d-106">Chiudere SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="cea3d-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="cea3d-107">Nel computer locale, rimuovere tutti i file trovati in ognuna delle cartelle seguenti.</span><span class="sxs-lookup"><span data-stu-id="cea3d-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="cea3d-108">Extensions\Cache del server%APPDATA%\Microsoft\Web</span><span class="sxs-lookup"><span data-stu-id="cea3d-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="cea3d-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="cea3d-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="cea3d-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="cea3d-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="cea3d-111">Aprire SharePoint Designer 2013 e immettere di nuovo l'account per verificare se funziona.</span><span class="sxs-lookup"><span data-stu-id="cea3d-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="cea3d-112">Passaggio 3: [abilitare l'autenticazione moderna per Office 2013 nei dispositivi Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="cea3d-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="cea3d-113">Passaggio 4: gli amministratori dovranno **consentire lo script personalizzato** nelle impostazioni dell'interfaccia di amministrazione di SharePoint per consentire la connessione a SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="cea3d-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="cea3d-114">Per ulteriori informazioni, vedere [Consenti o Impedisci lo script personalizzato](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="cea3d-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


