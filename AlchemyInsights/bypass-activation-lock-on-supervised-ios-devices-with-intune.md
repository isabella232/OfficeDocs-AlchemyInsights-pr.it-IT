---
title: Ignorare blocco di attivazione nei dispositivi iOS supervisionati con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397733"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="3e187-102">Ignorare blocco di attivazione nei dispositivi iOS supervisionati con Intune</span><span class="sxs-lookup"><span data-stu-id="3e187-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="3e187-103">La possibilità di ignorare il blocco di attivazione su dispositivi iOS semplifica il ripristino in scenari in cui un utente abilita il blocco di attivazione su un dispositivo aziendale e poi lascia l'azienda.</span><span class="sxs-lookup"><span data-stu-id="3e187-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="3e187-104">I prerequisiti per ignorare un blocco di attivazione includono:</span><span class="sxs-lookup"><span data-stu-id="3e187-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="3e187-105">Il dispositivo è “supervisionato”.</span><span class="sxs-lookup"><span data-stu-id="3e187-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="3e187-106">Il blocco di attivazione viene abilitato con i criteri di restrizione dei dispositivi iOS in Intune.</span><span class="sxs-lookup"><span data-stu-id="3e187-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="3e187-107">Inoltre, quando si ignora un blocco di attivazione, è necessario:</span><span class="sxs-lookup"><span data-stu-id="3e187-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="3e187-108">Essere in possesso materiale del dispositivo che si eliminerà.</span><span class="sxs-lookup"><span data-stu-id="3e187-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="3e187-109">Copiare il codice prima di eseguire la cancellazione.</span><span class="sxs-lookup"><span data-stu-id="3e187-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="3e187-110">**Nota:** il codice cancellazione non fa distinzione tra maiuscole e minuscole, quindi i caratteri “-” non sono necessari.</span><span class="sxs-lookup"><span data-stu-id="3e187-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="3e187-111">Per informazioni dettagliate, vedere [Ignorare il blocco di attivazione nei dispositivi iOS supervisionati con Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="3e187-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="3e187-112">**Domande frequenti**</span><span class="sxs-lookup"><span data-stu-id="3e187-112">**FAQ**</span></span>

<span data-ttu-id="3e187-113">D: **Ho eseguito un'azione da remoto per rimuovere i dati aziendali da un dispositivo, che ora è bloccato e il suo stato è in sospeso.**</span><span class="sxs-lookup"><span data-stu-id="3e187-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="3e187-114">R: Per completare correttamente un'azione da remoto, il dispositivo di destinazione deve essere online e integro.</span><span class="sxs-lookup"><span data-stu-id="3e187-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="3e187-115">Nelle situazioni seguenti, l'azione da remoto resta in sospeso per 30 giorni o finché il dispositivo non riconosce il comando quando il dispositivo:</span><span class="sxs-lookup"><span data-stu-id="3e187-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="3e187-116">Non ha connettività.</span><span class="sxs-lookup"><span data-stu-id="3e187-116">Does not have connectivity.</span></span>
- <span data-ttu-id="3e187-117">Perde lo stato di gestione con Intune.</span><span class="sxs-lookup"><span data-stu-id="3e187-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="3e187-118">Se ritieni che un dispositivo non sia più connesso e non rimuova i dati aziendali, selezionare Elimina.</span><span class="sxs-lookup"><span data-stu-id="3e187-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="3e187-119">L'eliminazione rimuove il registro del dispositivo in modo che non venga più visualizzato nell'elenco Intune dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="3e187-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="3e187-120">Per riattivare il dispositivo, è necessario che l'utente lo registri nuovamente.</span><span class="sxs-lookup"><span data-stu-id="3e187-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="3e187-121">D: **Perché alcune azioni remote non sono disponibili?**</span><span class="sxs-lookup"><span data-stu-id="3e187-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="3e187-122">R: Non tutte le piattaforme supportano tutte le azioni del dispositivo remoto.</span><span class="sxs-lookup"><span data-stu-id="3e187-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="3e187-123">Le azioni da remoto riportate di seguito sono specifiche per ciascuna piattaforma.</span><span class="sxs-lookup"><span data-stu-id="3e187-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="3e187-124">Ignora blocco attivazione (solo per iOS)</span><span class="sxs-lookup"><span data-stu-id="3e187-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="3e187-125">Fresh Start (solo per Windows)</span><span class="sxs-lookup"><span data-stu-id="3e187-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="3e187-126">Modalità smarrito (solo per iOS)</span><span class="sxs-lookup"><span data-stu-id="3e187-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="3e187-127">Individuare il dispositivo (solo per iOS)</span><span class="sxs-lookup"><span data-stu-id="3e187-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="3e187-128">Riavviare (solo per Windows)</span><span class="sxs-lookup"><span data-stu-id="3e187-128">Restart (Windows only)</span></span>

<span data-ttu-id="3e187-129">Per altre informazioni su ogni azione, vedere [Azioni del dispositivo disponibili](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="3e187-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>