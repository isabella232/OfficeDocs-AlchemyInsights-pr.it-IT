---
title: Sito moderno come sito radice
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057731"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="26c51-102">Sito moderno come sito radice</span><span class="sxs-lookup"><span data-stu-id="26c51-102">Modern site as root site</span></span>

<span data-ttu-id="26c51-103">I clienti di [release di destinazione](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) possono ora abilitare la moderna esperienza del sito di comunicazione nel sito radice classico del tenant di SharePoint.</span><span class="sxs-lookup"><span data-stu-id="26c51-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="26c51-104">Questa funzionalità può essere attivata eseguendo un semplice cmdlet di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="26c51-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="26c51-105">Per l'esecuzione corretta dei comandi di PowerShell, il sito radice avrà una nuova Home page del sito di comunicazione.</span><span class="sxs-lookup"><span data-stu-id="26c51-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="26c51-106">Informazioni dettagliate sul cmdlet e sui requisiti di funzionalità di PowerShell sono disponibili nell'articolo [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="26c51-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="26c51-107">In questo modo, per impostazione predefinita, verranno implementati i clienti di release mirati all'inizio di maggio 2019 e il lancio sarà disponibile in tutto il mondo entro la fine del 2019 giugno.</span><span class="sxs-lookup"><span data-stu-id="26c51-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="26c51-108">Continuare a fare riferimento al [centro messaggi](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) per altre nuove funzionalità con Modern.</span><span class="sxs-lookup"><span data-stu-id="26c51-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="26c51-109">**Importante**: non eliminare il sito radice classico per creare un sito di comunicazione moderno.</span><span class="sxs-lookup"><span data-stu-id="26c51-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="26c51-110">Questo non è supportato da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="26c51-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="26c51-111">L'eliminazione del sito radice renderà tutti i siti di SharePoint dell'organizzazione inaccessibili a tutti gli utenti, fino a quando non si ripristina il sito o si crea un nuovo sito nello stesso URL.</span><span class="sxs-lookup"><span data-stu-id="26c51-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 