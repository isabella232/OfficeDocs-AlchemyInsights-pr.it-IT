---
title: File su richiesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745302"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="79e67-102">Configurare File su richiesta</span><span class="sxs-lookup"><span data-stu-id="79e67-102">Configure Files On-Demand</span></span>

<span data-ttu-id="79e67-103">La funzionalità File di OneDrive su richiesta consente di accedere a tutti i file di OneDrive senza doverli scaricare tutti occupando spazio di archiviazione nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79e67-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="79e67-104">Per configurare File su richiesta nel PC:</span><span class="sxs-lookup"><span data-stu-id="79e67-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="79e67-105">Selezionare l'icona della nuvola bianca o blu di **OneDrive** nell'area di notifica della barra delle applicazioni di Windows.</span><span class="sxs-lookup"><span data-stu-id="79e67-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="79e67-106">Selezionare l'icona dell'ingranaggio di **Guida e impostazioni** e quindi **Impostazioni**.</span><span class="sxs-lookup"><span data-stu-id="79e67-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="79e67-107">Nella scheda **Impostazioni** selezionare la casella **Risparmia spazio e scarica i file quando li usi**.</span><span class="sxs-lookup"><span data-stu-id="79e67-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="79e67-108">È anche possibile configurare File su richiesta con il registro di sistema.</span><span class="sxs-lookup"><span data-stu-id="79e67-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="79e67-109">Se si disabilita questa impostazione, gli utenti di Windows 10 ricevono lo stesso comportamento di sincronizzazione degli utenti delle versioni precedenti di Windows e non sono in grado di attivare File su richiesta.</span><span class="sxs-lookup"><span data-stu-id="79e67-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="79e67-110">Se non si configura l'impostazione, gli utenti possono attivare o disattivare File su richiesta a piacimento.</span><span class="sxs-lookup"><span data-stu-id="79e67-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="79e67-111">L'abilitazione di questo criterio imposta il valore della chiave del Registro di sistema seguente su 1.</span><span class="sxs-lookup"><span data-stu-id="79e67-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="79e67-112">La disabilitazione di questo criterio imposta il valore della seguente chiave del registro di sistema su 0.</span><span class="sxs-lookup"><span data-stu-id="79e67-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="79e67-113">Se l'opzione File su richiesta non è visualizzata nelle Impostazioni, verificare che il tipo di avvio del servizio "Driver filtro dei file di Windows Cloud" sia impostato su 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="79e67-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="79e67-114">L'abilitazione di questo criterio imposta il valore della seguente chiave del registro di sistema su 2.</span><span class="sxs-lookup"><span data-stu-id="79e67-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`