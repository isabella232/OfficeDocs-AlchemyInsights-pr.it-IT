---
title: Termini mancanti dall'archivio termini di SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766857"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="73875-102">Abilitazione della crittografia BitLocker con Intune</span><span class="sxs-lookup"><span data-stu-id="73875-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="73875-103">I criteri di protezione dell'endpoint di Intune possono essere utilizzati per configurare le impostazioni di crittografia di Boitlocker per i dispositivi Windows come descritto in: impostazioni di Windows10 (e versioni successive) per proteggere i dispositivi tramite Intune</span><span class="sxs-lookup"><span data-stu-id="73875-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="73875-104">È necessario tenere presente che molti dispositivi più recenti che eseguono Windows 10 supportano la crittografia automatica di BitLocker che viene attivata senza l'applicazione del criterio MDM.</span><span class="sxs-lookup"><span data-stu-id="73875-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="73875-105">Questo può influire sull'applicazione dei criteri se non sono configurate impostazioni predefinite.</span><span class="sxs-lookup"><span data-stu-id="73875-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="73875-106">Per ulteriori informazioni, vedere FAQ.</span><span class="sxs-lookup"><span data-stu-id="73875-106">See FAQ for more detail.</span></span>


<span data-ttu-id="73875-107">Domande  frequenti Q: quali edizioni di Windows supportano la crittografia dei dispositivi utilizzando il criterio di protezione di endpoint?</span><span class="sxs-lookup"><span data-stu-id="73875-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="73875-108"> A: le impostazioni dei criteri di protezione dell'endpoint di Intune vengono implementate tramite il CSP di BitLocker.</span><span class="sxs-lookup"><span data-stu-id="73875-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="73875-109">Non tutte le edizioni o le build di Windows supportano il CSP di BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="73875-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="73875-110">In questo momento le edizioni di Windows: Enterprise; Sono supportate l'istruzione, la telefonia mobile, l'Enterprise Mobile e la Professional (dalla Build 1809 e versioni successive).</span><span class="sxs-lookup"><span data-stu-id="73875-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="73875-111">D: se un dispositivo è già crittografato con BitLocker utilizzando le impostazioni predefinite del sistema operativo per il metodo di crittografia e la forza di cifratura (XTS-AES-128), l'applicazione di un criterio con impostazioni diverse attiva automaticamente la ricrittografia dell'unità con le nuove impostazioni?</span><span class="sxs-lookup"><span data-stu-id="73875-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="73875-112">R: No.</span><span class="sxs-lookup"><span data-stu-id="73875-112">A: No.</span></span> <span data-ttu-id="73875-113">Per applicare le nuove impostazioni di crittografia, è necessario innanzitutto decrittografare l'unità.</span><span class="sxs-lookup"><span data-stu-id="73875-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="73875-114">Nota per i dispositivi in fase di registrazione con il pilota automatico la crittografia automatica che si verificherà durante la configurazione guidata non viene attivata fino a quando non viene valutato il criterio di Intune che consente di utilizzare le impostazioni basate sui criteri al posto dei valori predefiniti del sistema operativo.</span><span class="sxs-lookup"><span data-stu-id="73875-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="73875-115">D se un dispositivo viene crittografato a causa dell'applicazione dei criteri di Intune, la crittografia viene decrittografata quando il criterio viene rimosso?</span><span class="sxs-lookup"><span data-stu-id="73875-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="73875-116">A: la rimozione dei criteri correlati alla crittografia non comporta la decrittografia delle unità configurate.</span><span class="sxs-lookup"><span data-stu-id="73875-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="73875-117">D: perché i criteri di conformità di Intune mostrano che il dispositivo non ha "abilitato BitLocker" ma lo è?</span><span class="sxs-lookup"><span data-stu-id="73875-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="73875-118">A: l'impostazione "BitLocker Enabled" in Intune Compliance Policy utilizza il client di certificazione integrità dispositivo di Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="73875-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="73875-119">Questo client misura solo lo stato del dispositivo al momento dell'avvio.</span><span class="sxs-lookup"><span data-stu-id="73875-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="73875-120">Pertanto, se un dispositivo non è stato riavviato dopo che è stata completata la crittografia BitLocker, il servizio client DHA non segnalerà BitLocker come attivo.</span><span class="sxs-lookup"><span data-stu-id="73875-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>