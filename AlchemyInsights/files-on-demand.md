---
title: File su richiesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 846cda97ccd52fcb43ae4a44f73deeaaa6dc093d
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406582"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="724f8-102">Configurare File su richiesta</span><span class="sxs-lookup"><span data-stu-id="724f8-102">Configure Files On-Demand</span></span>

<span data-ttu-id="724f8-103">La funzionalità File di OneDrive su richiesta consente di accedere a tutti i file di OneDrive senza doverli scaricare tutti occupando spazio di archiviazione nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="724f8-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="724f8-104">Per configurare File su richiesta nel PC:</span><span class="sxs-lookup"><span data-stu-id="724f8-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="724f8-105">Selezionare l'icona della nuvola bianca o blu di **OneDrive** nell'area di notifica della barra delle applicazioni di Windows.</span><span class="sxs-lookup"><span data-stu-id="724f8-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="724f8-106">Selezionare l'icona dell'ingranaggio di **Guida e impostazioni** e quindi **Impostazioni**.</span><span class="sxs-lookup"><span data-stu-id="724f8-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="724f8-107">Nella scheda **Impostazioni** selezionare la casella **Risparmia spazio e scarica i file quando li usi**.</span><span class="sxs-lookup"><span data-stu-id="724f8-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="724f8-108">È anche possibile configurare File su richiesta con il registro di sistema.</span><span class="sxs-lookup"><span data-stu-id="724f8-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="724f8-109">Se si disabilita questa impostazione, gli utenti di Windows 10 ricevono lo stesso comportamento di sincronizzazione degli utenti delle versioni precedenti di Windows e non sono in grado di attivare File su richiesta.</span><span class="sxs-lookup"><span data-stu-id="724f8-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="724f8-110">Se non si configura l'impostazione, gli utenti possono attivare o disattivare File su richiesta a piacimento.</span><span class="sxs-lookup"><span data-stu-id="724f8-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="724f8-111">L'abilitazione di questo criterio imposta il valore della chiave del Registro di sistema seguente su 1.</span><span class="sxs-lookup"><span data-stu-id="724f8-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="724f8-112">La disabilitazione di questo criterio imposta il valore della seguente chiave del registro di sistema su 0.</span><span class="sxs-lookup"><span data-stu-id="724f8-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="724f8-113">Se l'opzione File su richiesta non è visualizzata nelle Impostazioni, verificare che il tipo di avvio del servizio "Driver filtro dei file di Windows Cloud" sia impostato su 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="724f8-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="724f8-114">L'abilitazione di questo criterio imposta il valore della seguente chiave del registro di sistema su 2.</span><span class="sxs-lookup"><span data-stu-id="724f8-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`