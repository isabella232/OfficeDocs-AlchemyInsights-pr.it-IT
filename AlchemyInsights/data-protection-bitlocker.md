---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908714"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="1e842-102">Abilitazione della crittografia BitLocker con Intune</span><span class="sxs-lookup"><span data-stu-id="1e842-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="1e842-103">I criteri di protezione dell'endpoint di Intune possono essere utilizzati per configurare le impostazioni di crittografia di BitLocker per i dispositivi Windows.</span><span class="sxs-lookup"><span data-stu-id="1e842-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="1e842-104">Per ulteriori informazioni, vedere [impostazioni di Windows 10 (e versioni successive) per proteggere i dispositivi che utilizzano Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="1e842-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="1e842-105">È necessario tenere presente che molti dispositivi più recenti che eseguono Windows 10 supportano la crittografia automatica di BitLocker, che viene attivata senza l'applicazione del criterio MDM.</span><span class="sxs-lookup"><span data-stu-id="1e842-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="1e842-106">Questo può influire sull'applicazione dei criteri se sono configurate impostazioni non predefinite.</span><span class="sxs-lookup"><span data-stu-id="1e842-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="1e842-107">Per ulteriori informazioni, vedere le domande frequenti seguenti.</span><span class="sxs-lookup"><span data-stu-id="1e842-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="1e842-108">Per informazioni sulla risoluzione dei problemi relativi a BitLocker, vedere risolvere i problemi [relativi ai criteri di BitLocker in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="1e842-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="1e842-109">**Domande frequenti**</span><span class="sxs-lookup"><span data-stu-id="1e842-109">**FAQ**</span></span>

 <span data-ttu-id="1e842-110">D: quali edizioni di Windows supportano la crittografia del dispositivo utilizzando i criteri di protezione di endpoint?</span><span class="sxs-lookup"><span data-stu-id="1e842-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="1e842-111">A: le impostazioni dei criteri di protezione dell'endpoint di Intune vengono implementate tramite il [CSP di BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="1e842-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="1e842-112">Non tutte le edizioni o le build di Windows supportano il CSP di BitLocker.</span><span class="sxs-lookup"><span data-stu-id="1e842-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="1e842-113">In questo momento sono supportate le seguenti edizioni di Windows: Enterprise, Education, mobile, Mobile Enterprise e Professional (Build 1809 e versioni successive).</span><span class="sxs-lookup"><span data-stu-id="1e842-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="1e842-114">D: se un dispositivo è già crittografato con BitLocker utilizzando le impostazioni predefinite del sistema operativo per il metodo di crittografia e la forza di cifratura (XTS-AES-128), l'applicazione di un criterio con impostazioni diverse attiverà automaticamente la ricrittografia dell'unità con le nuove impostazioni?</span><span class="sxs-lookup"><span data-stu-id="1e842-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="1e842-115">R: No.</span><span class="sxs-lookup"><span data-stu-id="1e842-115">A: No.</span></span> <span data-ttu-id="1e842-116">Per applicare le nuove impostazioni di crittografia, è necessario prima decrittografare l'unità.</span><span class="sxs-lookup"><span data-stu-id="1e842-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="1e842-117">**Nota:** Per i dispositivi che vengono registrati con Autopilot, la crittografia automatica che si verificherà durante la configurazione guidata non viene attivata fino a quando non viene valutato il criterio di Intune, che consente di utilizzare le impostazioni basate sui criteri al posto dei valori predefiniti del sistema operativo.</span><span class="sxs-lookup"><span data-stu-id="1e842-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="1e842-118">D: se un dispositivo viene crittografato a causa dell'applicazione dei criteri di Intune, verrà decrittografato quando il criterio viene rimosso?</span><span class="sxs-lookup"><span data-stu-id="1e842-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="1e842-119">A: la rimozione dei criteri correlati alla crittografia non comporta la decrittografia delle unità configurate.</span><span class="sxs-lookup"><span data-stu-id="1e842-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="1e842-120">D: perché i criteri di conformità di Intune mostrano che il dispositivo non dispone di BitLocker abilitato, anche se lo è?</span><span class="sxs-lookup"><span data-stu-id="1e842-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="1e842-121">A: l'impostazione "BitLocker Enabled" nel criterio di conformità di Intune utilizza il client di attestazione integrità del dispositivo di Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="1e842-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="1e842-122">Questo client misura solo lo stato del dispositivo al momento dell'avvio.</span><span class="sxs-lookup"><span data-stu-id="1e842-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="1e842-123">Pertanto, se un dispositivo non è stato riavviato dopo che la crittografia BitLocker è stata completata, il servizio client DHA non segnalerà BitLocker come attivo.</span><span class="sxs-lookup"><span data-stu-id="1e842-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 