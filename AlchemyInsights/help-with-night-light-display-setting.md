---
title: Guida per l’impostazione della luce notturna
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123080"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="4457f-102">Guida per l’impostazione della luce notturna</span><span class="sxs-lookup"><span data-stu-id="4457f-102">Help with the night light display setting</span></span>

<span data-ttu-id="4457f-103">Per altre informazioni sulle impostazioni della luce notturna, [impostare l'orario notturno in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="4457f-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="4457f-104">Se le opzioni per la luce notturna sono disattivate in Impostazioni, controllare il driver video:</span><span class="sxs-lookup"><span data-stu-id="4457f-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="4457f-105">Fare clic sulla casella di ricerca della barra delle applicazioni e digitare **Gestione dispositivi**, quindi selezionare **Gestione dispositivi** nei risultati della ricerca.</span><span class="sxs-lookup"><span data-stu-id="4457f-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="4457f-106">Espandere **schede video**.</span><span class="sxs-lookup"><span data-stu-id="4457f-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="4457f-107">Purtroppo, la caratteristica Luce notturna non è disponibile se il dispositivo usa un driver DisplayLink o un driver video Basic.</span><span class="sxs-lookup"><span data-stu-id="4457f-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="4457f-108">La caratteristica Luce notturna usa la recente tecnologia di grafica, quindi potrebbe essere necessario aggiornare il driver video:</span><span class="sxs-lookup"><span data-stu-id="4457f-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="4457f-109">Controllare la disponibilità di aggiornamenti andando a **Start** > **Impostazioni** > **Aggiornamento e sicurezza** > **Windows Update** > **Controlla aggiornamenti**.</span><span class="sxs-lookup"><span data-stu-id="4457f-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="4457f-110">OPPURE</span><span class="sxs-lookup"><span data-stu-id="4457f-110">OR</span></span>

- <span data-ttu-id="4457f-111">Visitare il sito Web del supporto del produttore hardware per scaricare e installare manualmente i driver video più recenti.</span><span class="sxs-lookup"><span data-stu-id="4457f-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="4457f-112">Ripristinare la luce notturna nel Registro di sistema</span><span class="sxs-lookup"><span data-stu-id="4457f-112">Reset night light in the registry</span></span>

<span data-ttu-id="4457f-113">Se l'aggiornamento del driver video non funziona, potrebbe essere necessario ripristinare la luce notturna nel Registro di sistema.</span><span class="sxs-lookup"><span data-stu-id="4457f-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="4457f-114">**Attenzione:** questa procedura di risoluzione dei problemi è consigliata solo per gli utenti avanzati.</span><span class="sxs-lookup"><span data-stu-id="4457f-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="4457f-115">L'errata modifica del Registro di sistema può causare seri problemi.</span><span class="sxs-lookup"><span data-stu-id="4457f-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="4457f-116">Per una maggiore protezione, eseguire un backup del Registro di sistema prima di modificarlo in modo da poterlo ripristinare in cso di problemi.</span><span class="sxs-lookup"><span data-stu-id="4457f-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="4457f-117">Nella casella di ricerca digitare **regedit** e quindi selezionare **Editor del Registro di sistema** nei risultati della ricerca.</span><span class="sxs-lookup"><span data-stu-id="4457f-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="4457f-118">Passare alla seguente chiave del Registro di sistema:</span><span class="sxs-lookup"><span data-stu-id="4457f-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="4457f-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="4457f-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="4457f-120">Esportare ed eliminare la sottochiave seguente:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="4457f-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="4457f-121">Esportare ed eliminare la sottochiave seguente:xport and then delete the following subkey:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="4457f-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="4457f-122">Riavviare Windows e verificare se sono disponibili le opzioni per la luce notturna.</span><span class="sxs-lookup"><span data-stu-id="4457f-122">Restart Windows and verify if the night light options are available.</span></span>


