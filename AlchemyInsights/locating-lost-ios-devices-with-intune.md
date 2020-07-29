---
title: Individuazione di dispositivi iOS smarriti con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434595"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="03449-102">Individuazione di dispositivi iOS smarriti con Intune</span><span class="sxs-lookup"><span data-stu-id="03449-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="03449-103">L'abilitazione della Modalità smarrito su un dispositivo iOS consente a un amministratore di avere un messaggio e un numero di telefono di contatto visualizzati nella schermata di blocco.</span><span class="sxs-lookup"><span data-stu-id="03449-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="03449-104">Dopo l'abilitazione della Modalità smarrito, l'amministratore può usare l'azione Individua dispositivo per identificare la posizione fisica del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03449-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="03449-105">L'azione Individua dispositivo in Intune funziona con i dispositivi iOS per mostrare la posizione di un dispositivo specifico su una mappa.</span><span class="sxs-lookup"><span data-stu-id="03449-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="03449-106">Con questa azione è necessario che il dispositivo iOS sia in:</span><span class="sxs-lookup"><span data-stu-id="03449-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="03449-107">Modalità supervisione</span><span class="sxs-lookup"><span data-stu-id="03449-107">Supervised mode</span></span>
- <span data-ttu-id="03449-108">Modalità smarrito</span><span class="sxs-lookup"><span data-stu-id="03449-108">Lost mode</span></span>

<span data-ttu-id="03449-109">Per altre informazioni, vedere [Abilitare la Modalità smarrito nei dispositivi iOS/iPadOS con Intune](https://docs.microsoft.com/intune/device-lost-mode) e [Individuare i dispositivi iOS/iPadOS smarriti o rubati con Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="03449-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="03449-110">**Domande frequenti**</span><span class="sxs-lookup"><span data-stu-id="03449-110">**FAQ**</span></span>

<span data-ttu-id="03449-111">D: Ho eseguito un'azione da remoto per rimuovere i dati aziendali da un dispositivo, che ora è bloccato e il suo stato è in sospeso.</span><span class="sxs-lookup"><span data-stu-id="03449-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="03449-112">R: Per completare correttamente un'azione da remoto, il dispositivo di destinazione deve essere online e integro.</span><span class="sxs-lookup"><span data-stu-id="03449-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="03449-113">Nelle situazioni seguenti, l'azione da remoto resta in sospeso per 30 giorni o finché il dispositivo non riconosce il comando:</span><span class="sxs-lookup"><span data-stu-id="03449-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="03449-114">Quando il dispositivo non ha connettività</span><span class="sxs-lookup"><span data-stu-id="03449-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="03449-115">Quando il dispositivo perde lo stato di gestione con Intune</span><span class="sxs-lookup"><span data-stu-id="03449-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="03449-116">Se ritieni che un dispositivo non sia più connesso e non sia in grado di rimuovere i dati aziendali, selezionare Elimina.</span><span class="sxs-lookup"><span data-stu-id="03449-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="03449-117">L'eliminazione rimuove il registro del dispositivo in modo che non venga più visualizzato nell'elenco Intune dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="03449-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="03449-118">Se il dispositivo diventa nuovamente attivo, l'utente dovrà registrarlo di nuovo.</span><span class="sxs-lookup"><span data-stu-id="03449-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="03449-119">D: Perché alcune azioni remote non sono disponibili?</span><span class="sxs-lookup"><span data-stu-id="03449-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="03449-120">R: Non tutte le piattaforme supportano tutte le azioni del dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="03449-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="03449-121">Le azioni remote seguenti sono specifiche per determinate piattaforme, quindi sono disponibili solo per tali piattaforme.</span><span class="sxs-lookup"><span data-stu-id="03449-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="03449-122">Ignora blocco attivazione (solo per iOS)</span><span class="sxs-lookup"><span data-stu-id="03449-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="03449-123">Fresh Start (solo per Windows)</span><span class="sxs-lookup"><span data-stu-id="03449-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="03449-124">Modalità smarrito (solo per iOS)</span><span class="sxs-lookup"><span data-stu-id="03449-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="03449-125">Individuare il dispositivo (solo per iOS)</span><span class="sxs-lookup"><span data-stu-id="03449-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="03449-126">Riavviare (solo per Windows)</span><span class="sxs-lookup"><span data-stu-id="03449-126">Restart (Windows only)</span></span>

<span data-ttu-id="03449-127">Per altre informazioni su ogni azione, vedere [Azioni del dispositivo disponibili](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="03449-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>