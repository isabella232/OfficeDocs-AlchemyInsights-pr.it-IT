---
title: Pulizia automatica di dispositivi non aggiornati in Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505203"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="e7fb6-102">Pulizia automatica di dispositivi non aggiornati in Intune</span><span class="sxs-lookup"><span data-stu-id="e7fb6-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="e7fb6-103">Intune consente all'amministratore di configurare un intervallo di tempo compreso tra 90 e 270 giorni, dopo il quale i dispositivi non aggiornati verranno rimossi dal servizio.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="e7fb6-104">Questa impostazione è estesa all'intera organizzazione e, una volta attivata, diventa effettiva immediatamente.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="e7fb6-105">Qualsiasi dispositivo non archiviato nel server di Intune per un periodo superiore a quello impostato verrà eliminato definitivamente.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="e7fb6-106">**Nota** Solo gli oggetti dei dispositivi MDM sono idonei per questa azione di pulizia.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="e7fb6-107">Sono esclusi solo gli oggetti dei dispositivi EAS.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="e7fb6-108">Per altre informazioni su quando un dispositivo diventa idoneo per l'eliminazione in base all'opzione di pulizia del dispositivo e al relativo "stato":</span><span class="sxs-lookup"><span data-stu-id="e7fb6-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="e7fb6-109">Impostazione: **Eliminare dispositivi dopo l'ultima data di archiviazione: Sì (un valore specifico (N) di giorni)**</span><span class="sxs-lookup"><span data-stu-id="e7fb6-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="e7fb6-110">In base al valore (N) configurato nell'impostazione, il servizio Intune elimina il dispositivo dopo il numero di giorni specificato dall'ultima archiviazione.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="e7fb6-111">Impostazioni: **Eliminare dispositivi dopo l'ultima data di archiviazione: No**</span><span class="sxs-lookup"><span data-stu-id="e7fb6-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="e7fb6-112">180 giorni dopo la scadenza del certificato del dispositivo e in mancanza del suo rinnovo, il dispositivo viene eliminato.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="e7fb6-113">**Nota** In entrambi i casi, il dispositivo deve essere registrato correttamente in Intune.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="e7fb6-114">La registrazione si verifica durante la prima archiviazione del dispositivo con il servizio Intune.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="e7fb6-115">Se un dispositivo viene iscritto correttamente con Intune ma è registrato in Intune, il dispositivo verrà eliminato 270 giorni dopo l'iscrizione.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="e7fb6-116">(90 giorni in cui è possibile selezionare il dispositivo come revocato e altri 180 giorni per eliminare il record.)</span><span class="sxs-lookup"><span data-stu-id="e7fb6-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="e7fb6-117">Attualmente non è presente alcun meccanismo nella console Intune per stabilire la data di scadenza della certificazione del dispositivo per qualsiasi dispositivo specifico.</span><span class="sxs-lookup"><span data-stu-id="e7fb6-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>