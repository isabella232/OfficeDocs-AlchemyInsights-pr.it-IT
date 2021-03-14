---
title: Rimuovere il servizio in background per Microsoft Search in Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753416"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="40f89-102">Rimuovere il servizio in background per Microsoft Search in Bing</span><span class="sxs-lookup"><span data-stu-id="40f89-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="40f89-103">Per rimuovere il servizio in background per Microsoft Search in Bing, è possibile provare i rimedi seguenti:</span><span class="sxs-lookup"><span data-stu-id="40f89-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="40f89-104">Per ripristinare le impostazioni originali del motore di ricerca, eseguire queste operazioni:</span><span class="sxs-lookup"><span data-stu-id="40f89-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="40f89-105">a.</span><span class="sxs-lookup"><span data-stu-id="40f89-105">a.</span></span> <span data-ttu-id="40f89-106">Disattivare l'opzione **Usa Bing come motore di ricerca predefinito[](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) impostando l’interruttore su Disattivato**.</span><span class="sxs-lookup"><span data-stu-id="40f89-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="40f89-107">b.</span><span class="sxs-lookup"><span data-stu-id="40f89-107">b.</span></span> <span data-ttu-id="40f89-108">[Accedere all'interfaccia di amministrazione di Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) e deselezionare l'impostazione che riguarda tutti gli utenti dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="40f89-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="40f89-109">Per rimuovere il servizio in background da un singolo dispositivo, eseguire queste attività:</span><span class="sxs-lookup"><span data-stu-id="40f89-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="40f89-110">a.</span><span class="sxs-lookup"><span data-stu-id="40f89-110">a.</span></span> <span data-ttu-id="40f89-111">Scegliere **Pannello di controllo > Programmi > Programmi e funzionalità**.</span><span class="sxs-lookup"><span data-stu-id="40f89-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="40f89-112">b.</span><span class="sxs-lookup"><span data-stu-id="40f89-112">b.</span></span> <span data-ttu-id="40f89-113">Fare clic con il pulsante destro del mouse su **Microsoft Search in Bing** nell'elenco dei programmi installati e quindi scegliere **Disinstalla**.</span><span class="sxs-lookup"><span data-stu-id="40f89-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="40f89-114">Per rimuovere il servizio in background da più dispositivi dell'organizzazione, accedere come amministratore ed eseguire il comando seguente in uno script:</span><span class="sxs-lookup"><span data-stu-id="40f89-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
