---
title: Inventario dispositivi Intune
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667882"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="b92e9-102">Inventario dispositivi Intune</span><span class="sxs-lookup"><span data-stu-id="b92e9-102">Intune Device Inventory</span></span>

<span data-ttu-id="b92e9-103">Il pannello Dispositivi fornisce all'amministratore informazioni dettagliate sui dispositivi gestiti in Intune per ogni dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b92e9-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="b92e9-104">Le informazioni visualizzate includono: hardware, applicazioni individuate, stato di conformità e stato di configurazione del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b92e9-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="b92e9-105">I dati di inventario per l'hardware e le applicazioni individuate vengono raccolti ogni sette giorni.</span><span class="sxs-lookup"><span data-stu-id="b92e9-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="b92e9-106">Le applicazioni e gli elementi specifici dell'hardware segnalato variano in base al sistema operativo del dispositivo e al fatto che il dispositivo sia di proprietà personale o aziendale.</span><span class="sxs-lookup"><span data-stu-id="b92e9-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="b92e9-107">Per altre informazioni, consultare [Vedere i dettagli del dispositivo in Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="b92e9-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="b92e9-108">**Domande frequenti**</span><span class="sxs-lookup"><span data-stu-id="b92e9-108">**FAQ**</span></span>

<span data-ttu-id="b92e9-109">D: non ricevo un elenco completo delle applicazioni presenti nei dispositivi Windows registrati in Intune.</span><span class="sxs-lookup"><span data-stu-id="b92e9-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="b92e9-110">Perché?</span><span class="sxs-lookup"><span data-stu-id="b92e9-110">Why not?</span></span>

<span data-ttu-id="b92e9-111">R: al momento, compaiono nell'elenco solo le app moderne per PC Windows 10 identificati come dispositivi aziendali.</span><span class="sxs-lookup"><span data-stu-id="b92e9-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="b92e9-112">Intune non raccoglie informazioni sulle app Win32 installate su questi dispositivi.</span><span class="sxs-lookup"><span data-stu-id="b92e9-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="b92e9-113">D: perché i numeri di telefono non vengono raccolti da tutti i dispositivi?</span><span class="sxs-lookup"><span data-stu-id="b92e9-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="b92e9-114">R: i telefoni categorizzati come dispositivi aziendali in Intune non vengono identificati con il numero di telefono completo quando, ad esempio, si esegue un report inventario di dispositivi mobili.</span><span class="sxs-lookup"><span data-stu-id="b92e9-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="b92e9-115">I numeri di telefono Bring-You-Own-Device sono sempre parzialmente mascherati da asterischi (\*\*\*\*) e mostrano solo le ultime quattro cifre.</span><span class="sxs-lookup"><span data-stu-id="b92e9-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>