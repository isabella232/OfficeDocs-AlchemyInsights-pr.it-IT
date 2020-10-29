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
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791298"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="b633f-102">Configurare File su richiesta</span><span class="sxs-lookup"><span data-stu-id="b633f-102">Configure Files On-Demand</span></span>

<span data-ttu-id="b633f-103">File di OneDrive su richiesta richiede [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (versione 1709 o successiva) o Windows Server 2019 e OneDrive build 17.3.7064.1005 o successiva.</span><span class="sxs-lookup"><span data-stu-id="b633f-103">OneDrive Files On-Demand requires [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (version 1709 or later) or Windows Server 2019 and OneDrive build 17.3.7064.1005 or later.</span></span>

<span data-ttu-id="b633f-104">La funzionalità File di OneDrive su richiesta consente di accedere a tutti i file di OneDrive senza doverli scaricare tutti occupando spazio di archiviazione nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b633f-104">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="b633f-105">Per configurare File su richiesta nel PC:</span><span class="sxs-lookup"><span data-stu-id="b633f-105">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="b633f-106">Selezionare l'icona della nuvola bianca o blu di **OneDrive** nell'area di notifica della barra delle applicazioni di Windows.</span><span class="sxs-lookup"><span data-stu-id="b633f-106">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="b633f-107">Selezionare l'icona dell'ingranaggio di **Guida e impostazioni** e quindi **Impostazioni** .</span><span class="sxs-lookup"><span data-stu-id="b633f-107">Select the **Help & Settings** gear icon > **Settings** .</span></span>
2. <span data-ttu-id="b633f-108">Nella scheda **Impostazioni** selezionare la casella **Risparmia spazio e scarica i file quando li usi** .</span><span class="sxs-lookup"><span data-stu-id="b633f-108">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="b633f-109">È anche possibile configurare File su richiesta con il registro di sistema.</span><span class="sxs-lookup"><span data-stu-id="b633f-109">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="b633f-110">Se si disabilita questa impostazione, gli utenti di Windows 10 ricevono lo stesso comportamento di sincronizzazione degli utenti delle versioni precedenti di Windows e non sono in grado di attivare File su richiesta.</span><span class="sxs-lookup"><span data-stu-id="b633f-110">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="b633f-111">Se non si configura l'impostazione, gli utenti possono attivare o disattivare File su richiesta a piacimento.</span><span class="sxs-lookup"><span data-stu-id="b633f-111">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="b633f-112">L'abilitazione di questo criterio imposta il valore della chiave del Registro di sistema seguente su 1.</span><span class="sxs-lookup"><span data-stu-id="b633f-112">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="b633f-113">La disabilitazione di questo criterio imposta il valore della seguente chiave del registro di sistema su 0.</span><span class="sxs-lookup"><span data-stu-id="b633f-113">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="b633f-114">Se l'opzione File su richiesta non è visualizzata nelle Impostazioni, verificare che il tipo di avvio del servizio "Driver filtro dei file di Windows Cloud" sia impostato su 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="b633f-114">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="b633f-115">L'abilitazione di questo criterio imposta il valore della seguente chiave del registro di sistema su 2.</span><span class="sxs-lookup"><span data-stu-id="b633f-115">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`