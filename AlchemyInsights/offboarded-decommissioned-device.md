---
title: Problemi con la rimozione di un dispositivo disattivato o rimosso dall'inventario dei dispositivi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/11/2021
ms.locfileid: "52319175"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="6cb15-102">Problemi con la rimozione di un dispositivo disattivato o rimosso dall'inventario dei dispositivi</span><span class="sxs-lookup"><span data-stu-id="6cb15-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="6cb15-103">Microsoft Defender for Endpoint attualmente non consente la rimozione manuale del record del dispositivo di un dispositivo offboarding o rimosso dall'inventario dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="6cb15-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="6cb15-104">Per motivi di sicurezza, il dispositivo rimane nel portale come record cronologico fino a 180 giorni.</span><span class="sxs-lookup"><span data-stu-id="6cb15-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="6cb15-105">Tuttavia, i dati del dispositivo vengono eliminati in base al periodo di conservazione configurato.</span><span class="sxs-lookup"><span data-stu-id="6cb15-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="6cb15-106">**Nota:** Un dispositivo disattivato o disattivato passa automaticamente allo stato **Inattivo** dopo sette giorni.</span><span class="sxs-lookup"><span data-stu-id="6cb15-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="6cb15-107">Inoltre, i dispositivi non attivi negli ultimi 30 giorni non vengono fattoriati nei dati che riflettono il punteggio di esposizione per la gestione delle minacce e delle vulnerabilità dell'organizzazione o il punteggio microsoft secure per i dispositivi.</span><span class="sxs-lookup"><span data-stu-id="6cb15-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="6cb15-108">Se ancora non vuoi visualizzare determinati dispositivi nella visualizzazione Inventario dispositivi, prova a inserire un tag del dispositivo per filtrare il dispositivo rimosso dalla visualizzazione Inventario dispositivi.</span><span class="sxs-lookup"><span data-stu-id="6cb15-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="6cb15-109">Per altre informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="6cb15-109">For more information, see:</span></span>

[<span data-ttu-id="6cb15-110">Dispositivi offboard dal servizio Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="6cb15-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="6cb15-111">Punteggio di esposizione nella gestione delle minacce e delle vulnerabilità</span><span class="sxs-lookup"><span data-stu-id="6cb15-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="6cb15-112">Risolvere i sensori non integri in Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="6cb15-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="6cb15-113">Come usare il tagging in modo efficace (parte 1)</span><span class="sxs-lookup"><span data-stu-id="6cb15-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="6cb15-114">Come usare il tagging in modo efficace (parte 2)</span><span class="sxs-lookup"><span data-stu-id="6cb15-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="6cb15-115">Come usare il tagging in modo efficace (parte 3)</span><span class="sxs-lookup"><span data-stu-id="6cb15-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




