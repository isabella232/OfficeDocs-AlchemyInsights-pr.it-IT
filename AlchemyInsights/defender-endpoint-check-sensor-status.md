---
title: Controllo dello stato del sensore di Defender per endpoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/24/2021
ms.locfileid: "52627244"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="c0162-102">Controllo dello stato del sensore di Defender per endpoint</span><span class="sxs-lookup"><span data-stu-id="c0162-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="c0162-103">Il riquadro **Dispositivi con problemi di sensore** si trova nel dashboard Operazioni di sicurezza.</span><span class="sxs-lookup"><span data-stu-id="c0162-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="c0162-104">Questo riquadro fornisce informazioni sulla capacità del singolo dispositivo di fornire dati sul sensore e comunicare con il servizio Defender per endpoint.</span><span class="sxs-lookup"><span data-stu-id="c0162-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="c0162-105">Segnala quanti dispositivi richiedono attenzione e aiuta a identificare i dispositivi problematici per intraprendere le azioni volte a correggere i problemi noti.</span><span class="sxs-lookup"><span data-stu-id="c0162-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="c0162-106">Due indicatori di stato nel riquadro forniscono informazioni sul numero di dispositivi che non segnalano correttamente al servizio:</span><span class="sxs-lookup"><span data-stu-id="c0162-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="c0162-107">**Configurazione non corretta** Dispositivi che potrebbero segnalare parzialmente i dati del sensore al servizio Defender per endpoint e contenere errori di configurazione da correggere.</span><span class="sxs-lookup"><span data-stu-id="c0162-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="c0162-108">**Inattivi** Dispositivi che hanno interrotto la segnalazione al servizio Defender per endpoint per più di sette giorni nell'ultimo mese.</span><span class="sxs-lookup"><span data-stu-id="c0162-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="c0162-109">Facendo clic su uno dei gruppi, si viene indirizzati all'elenco Dispositivi, filtrato in base alle scelte effettuate.</span><span class="sxs-lookup"><span data-stu-id="c0162-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="c0162-110">È possibile filtrare l'elenco Dispositivi in base allo stato di integrità come segue:</span><span class="sxs-lookup"><span data-stu-id="c0162-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="c0162-111">**Attivi** Dispositivi che segnalano attivamente al servizio Defender per endpoint.</span><span class="sxs-lookup"><span data-stu-id="c0162-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="c0162-112">**Configurazione non corretta** Dispositivi che potrebbero segnalare parzialmente i dati del sensore al servizio Defender per endpoint e contengono errori di configurazione da correggere.</span><span class="sxs-lookup"><span data-stu-id="c0162-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="c0162-113">Nei dispositivi non configurati correttamente possono verificarsi uno o più dei seguenti problemi:</span><span class="sxs-lookup"><span data-stu-id="c0162-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="c0162-114">Nessun dato del sensore: i dispositivi hanno smesso di inviare dati del sensore.</span><span class="sxs-lookup"><span data-stu-id="c0162-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="c0162-115">Il dispositivo può generare avvisi limitati.</span><span class="sxs-lookup"><span data-stu-id="c0162-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="c0162-116">Comunicazioni con problemi: sono presenti problemi di comunicazione con il dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c0162-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="c0162-117">L'invio di file per un'analisi approfondita, il blocco dei file, l'isolamento del dispositivo dalla rete e altre azioni che richiedono la comunicazione con il dispositivo potrebbero non funzionare.</span><span class="sxs-lookup"><span data-stu-id="c0162-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="c0162-118">**Inattivi** Dispositivi che hanno interrotto la segnalazione al servizio Defender per endpoint.</span><span class="sxs-lookup"><span data-stu-id="c0162-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="c0162-119">È possibile scaricare l'intero elenco in formato CSV usando la funzionalità Esporta.</span><span class="sxs-lookup"><span data-stu-id="c0162-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="c0162-120">Per altre informazioni, vedere [Controllare lo stato di integrità del sensore in Microsoft Defender per endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="c0162-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="c0162-121">Per altre informazioni su ciò che ha causato l'inattività o la configurazione non corretta di un dispositivo, vedere [Correggere i sensori non integri in Microsoft Defender per endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="c0162-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
