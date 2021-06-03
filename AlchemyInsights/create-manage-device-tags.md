---
title: Creare e gestire i tag dei dispositivi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721730"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="0e0b1-102">Creare e gestire i tag dei dispositivi</span><span class="sxs-lookup"><span data-stu-id="0e0b1-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="0e0b1-103">Aggiungere tag nei dispositivi per creare un'affiliazione a un gruppo logico.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="0e0b1-104">I tag del dispositivo supportano la mappatura corretta della rete, consentendo di collegare tag diversi per acquisire il contesto e consentire la creazione di elenchi dinamici come parte di un incidente.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="0e0b1-105">I tag possono essere usati come filtro nella visualizzazione Elenco dispositivi o per raggruppare i dispositivi.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="0e0b1-106">Per altre informazioni sul raggruppamento dei dispositivi, vedere [Creare e gestire i tag dei dispositivi](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="0e0b1-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="0e0b1-107">È possibile aggiungere tag nei dispositivi:</span><span class="sxs-lookup"><span data-stu-id="0e0b1-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="0e0b1-108">Usando il portale</span><span class="sxs-lookup"><span data-stu-id="0e0b1-108">Using the portal</span></span>

- <span data-ttu-id="0e0b1-109">Impostando un valore della chiave del Registro di sistema</span><span class="sxs-lookup"><span data-stu-id="0e0b1-109">Setting a registry key value</span></span>
 
<span data-ttu-id="0e0b1-110">**Nota:** potrebbe esserci latenza tra il momento in cui un tag viene aggiunto a un dispositivo e la sua disponibilità nell'elenco dei dispositivi e nella pagina del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="0e0b1-111">Per aggiungere tag del dispositivo usando l'API, vedere [Aggiungere o rimuovere l'API dei tag del dispositivo](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="0e0b1-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="0e0b1-112">Aggiungere e gestire i tag per i dispositivi tramite il portale</span><span class="sxs-lookup"><span data-stu-id="0e0b1-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="0e0b1-113">Selezionare il dispositivo in cui gestire i tag.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="0e0b1-114">È possibile selezionare o cercare un dispositivo in una delle seguenti visualizzazioni:</span><span class="sxs-lookup"><span data-stu-id="0e0b1-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="0e0b1-115">**Dashboard delle operazioni di sicurezza**: selezionare il nome del dispositivo dalla sezione Dispositivi principali con avvisi attivi.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="0e0b1-116">**Coda degli avvisi**: selezionare il nome del dispositivo accanto all'icona del dispositivo dalla coda degli avvisi.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="0e0b1-117">**Elenco dispositivi**: selezionare il nome del dispositivo nell'elenco dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="0e0b1-118">**Casella di ricerca**: selezionare Dispositivo dal menu a discesa e inserire il nome del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="0e0b1-119">È anche possibile accedere alla pagina di avviso tramite le visualizzazioni file e IP.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="0e0b1-120">Selezionare **Gestisci tag** dalla riga Azioni di risposta.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="0e0b1-121">Digitare per trovare o creare i tag.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-121">Type to find or create tags.</span></span>

<span data-ttu-id="0e0b1-122">I tag vengono aggiunti alla visualizzazione del dispositivo e si riflettono nella visualizzazione Elenco dispositivi.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="0e0b1-123">È quindi possibile usare il filtro dei tag per visualizzare l'elenco di dispositivi pertinente.</span><span class="sxs-lookup"><span data-stu-id="0e0b1-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="0e0b1-124">Per altre informazioni, vedere [Creare e gestire i tag dei dispositivi](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="0e0b1-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>