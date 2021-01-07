---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768821"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Abilitazione della crittografia BitLocker con Intune

 I criteri di protezione dell'endpoint di Intune possono essere utilizzati per configurare le impostazioni di crittografia di BitLocker per i dispositivi Windows. Per ulteriori informazioni, vedere [impostazioni di Windows 10 (e versioni successive) per proteggere i dispositivi che utilizzano Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
È necessario tenere presente che molti dispositivi più recenti che eseguono Windows 10 supportano la crittografia automatica di BitLocker, che viene attivata senza l'applicazione del criterio MDM. Questo può influire sull'applicazione dei criteri se sono configurate impostazioni non predefinite. Per ulteriori informazioni, vedere le domande frequenti seguenti.
 
Per informazioni sulla risoluzione dei problemi relativi a BitLocker, vedere risolvere i problemi [relativi ai criteri di BitLocker in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Domande frequenti**

D: quali edizioni di Windows supportano la crittografia del dispositivo utilizzando i criteri di protezione di endpoint?<br>
A: le impostazioni dei criteri di protezione dell'endpoint di Intune vengono implementate tramite il [CSP di BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Non tutte le edizioni o le build di Windows supportano il CSP di BitLocker. <br><br>

D: come è possibile abilitare BitLocker nei dispositivi senza richiedere l'interazione dell'utente finale?<br>
A: a condizione che vengano soddisfatti i prerequisiti necessari, è possibile abilitare BitLocker "Silent Encryption" tramite Intune. Vedere i dettagli dei requisiti del dispositivo e le impostazioni di criteri di esempio per abilitare la crittografia invisibile all'utente nel seguente documento: [abilitare la crittografia BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)in modo invisibile all'utente. <br><br>

D: se un dispositivo è già crittografato con BitLocker utilizzando le impostazioni predefinite del sistema operativo per il metodo di crittografia e la forza di cifratura (XTS-AES-128), l'applicazione di un criterio con impostazioni diverse attiverà automaticamente la ricrittografia dell'unità con le nuove impostazioni?<br>
R: No. Per applicare le nuove impostazioni di crittografia, è necessario prima decrittografare l'unità.<br><br>
**Nota:** Per i dispositivi che vengono registrati con Autopilot, la crittografia automatica che si verificherà durante la configurazione guidata non viene attivata fino a quando non viene valutato il criterio di Intune, che consente di utilizzare le impostazioni basate sui criteri al posto dei valori predefiniti del sistema operativo.
 
D: se un dispositivo viene crittografato a causa dell'applicazione dei criteri di Intune, verrà decrittografato quando il criterio viene rimosso?<br>
A: la rimozione dei criteri correlati alla crittografia non comporta la decrittografia delle unità configurate.
 
D: perché i criteri di conformità di Intune mostrano che il dispositivo non dispone di BitLocker abilitato, anche se lo è?<br>
A: l'impostazione "BitLocker Enabled" nel criterio di conformità di Intune utilizza il client di attestazione integrità del dispositivo di Windows (DHA). Questo client misura solo lo stato del dispositivo al momento dell'avvio. Pertanto, se un dispositivo non è stato riavviato dopo che la crittografia BitLocker è stata completata, il servizio client DHA non segnalerà BitLocker come attivo.
 
 