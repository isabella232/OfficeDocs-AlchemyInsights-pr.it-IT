---
title: Rimozione dei dati e cancellazione dei dispositivi in Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416317"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="5b5f9-102">Rimozione dei dati e cancellazione dei dispositivi in Intune</span><span class="sxs-lookup"><span data-stu-id="5b5f9-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="5b5f9-103">Le azioni remote Ritiro dispositivo e Cancellazione dispositivo possono essere utilizzate per rimuovere i dati aziendali gestiti da Intune o per eseguire il ripristino delle impostazioni predefinite e ripristinare il dispositivo alle impostazioni predefinite.</span><span class="sxs-lookup"><span data-stu-id="5b5f9-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="5b5f9-104">Accedere a Gestione dispositivi Microsoft 365 e passare a **Dispositivi** > **Tutti i dispositivi**.</span><span class="sxs-lookup"><span data-stu-id="5b5f9-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="5b5f9-105">Selezionare il dispositivo da cui cancellare i dati.</span><span class="sxs-lookup"><span data-stu-id="5b5f9-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="5b5f9-106">Selezionare il tipo di cancellazione remota da eseguire.</span><span class="sxs-lookup"><span data-stu-id="5b5f9-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="5b5f9-107">Il ritiro elimina solo le informazioni dell'organizzazione, mentre la cancellazione completa ripristina il dispositivo alle impostazioni predefinite.</span><span class="sxs-lookup"><span data-stu-id="5b5f9-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="5b5f9-108">Selezionare **Sì** per confermare.</span><span class="sxs-lookup"><span data-stu-id="5b5f9-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="5b5f9-109">Fino al completamento della cancellazione, lo stato azione del dispositivo sarà *Ritiro in sospeso*.</span><span class="sxs-lookup"><span data-stu-id="5b5f9-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="5b5f9-110">Una volta completata l'azione, il dispositivo mobile non verrà più visualizzato nell'elenco dei dispositivi gestiti.</span><span class="sxs-lookup"><span data-stu-id="5b5f9-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="5b5f9-111">Non è possibile rimuovere i dati aziendali dai dispositivi AGGIUNTI ad Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5b5f9-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="5b5f9-112">Per informazioni dettagliate sull'effetto delle azioni di ritiro e cancellazione, incluse le informazioni conservate ed eliminate, vedere la seguente documentazione:</span><span class="sxs-lookup"><span data-stu-id="5b5f9-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="5b5f9-113">[Rimuovere i dispositivi con la cancellazione, la disattivazione o l'annullamento della registrazione manuale del dispositivo](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="5b5f9-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="5b5f9-114">Come cancellare i dati aziendali solo dalle app gestite da Intune</span><span class="sxs-lookup"><span data-stu-id="5b5f9-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="5b5f9-115">[Cancellare tutti i dati da un dispositivo macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="5b5f9-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>