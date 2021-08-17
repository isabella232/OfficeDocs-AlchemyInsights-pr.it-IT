---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118598"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Abilitazione della crittografia Bitlocker con Intune

I criteri Endpoint Protection Intune possono essere usati per configurare le impostazioni di crittografia Bitlocker per Windows dispositivi. Per altre informazioni, vedi [Windows 10 (e versioni successive)](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)per proteggere i dispositivi con Intune.

Oltre ai criteri di Endpoint Protection, è disponibile anche un rapporto sulla crittografia che fornisce una visualizzazione più dettagliata dello stato di crittografia per i dispositivi. È possibile accedere a questo report dal portale MEM in **Dispositivi > Monitor** e quindi in Configurazione selezionare Report [crittografia](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport). 

Se si trova che Bitlocker non viene abilitato come previsto o che il profilo utilizzato per abilitare Bitlocker è in uno stato di errore, esaminare il report di crittografia per comprendere meglio il motivo per cui si verifica il comportamento.

Per informazioni dettagliate su come interpretare il report, inclusi i vari valori di stato della crittografia, vedi [Monitorare la crittografia dei dispositivi con Intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Tenere presente che molti dispositivi più nuovi che eseguono Windows 10 supportano la crittografia Bitlocker automatica, che viene attivata senza l'applicazione dei criteri MDM. Ciò può influire sull'applicazione dei criteri se sono configurate impostazioni non predefinite. Per ulteriori dettagli, vedere le domande frequenti seguenti.

Per informazioni sulla risoluzione dei problemi relativi a BitLocker, vedere [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Domande frequenti**

D: Quali edizioni di Windows supportano la crittografia dei dispositivi usando i criteri Endpoint Protection?<br>
A: Le impostazioni in Intune Endpoint Protection criteri vengono implementate usando il [CSP Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Non tutte le edizioni o le build di Windows supportano il CSP Bitlocker. <br><br>

D: Come è possibile abilitare Bitlocker nei dispositivi senza richiedere l'interazione dell'utente finale?<br>
A: Purché siano soddisfatti i prerequisiti necessari, è possibile abilitare Bitlocker "Silent Encryption" tramite Intune. Vedi i dettagli dei requisiti del dispositivo e le impostazioni dei criteri di esempio per abilitare la crittografia invisibile all'utente nel documento seguente: Abilitare in modo invisibile all'utente [Crittografia Bitlocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

D: Se un dispositivo è già crittografato con Bitlocker usando le impostazioni predefinite del sistema operativo per il metodo di crittografia e la forza di crittografia (XTS-AES-128), l'applicazione di un criterio con impostazioni diverse attiverà automaticamente una nuova crittografia dell'unità con le nuove impostazioni?<br>
R: no. Per applicare le nuove impostazioni di crittografia, l'unità deve prima essere decrittografata.<br><br>
**Nota:** Per i dispositivi registrati con Autopilot, la crittografia automatica che si verificherebbe durante la configurazione guidata non viene attivata fino a quando non viene valutato il criterio di Intune, che consente di usare le impostazioni basate su criteri al posto delle impostazioni predefinite del sistema operativo.
 
D: Se un dispositivo viene crittografato come risultato dell'applicazione dei criteri di Intune, verrà decrittografato quando tale criterio viene rimosso?<br>
A: La rimozione dei criteri relativi alla crittografia NON comporta la decrittografia delle unità configurate.
 
D: Perché i criteri di conformità di Intune mostrano che nel dispositivo non è abilitato Bitlocker, anche se lo è?<br>
A: L'impostazione "Bitlocker abilitato" nei criteri di conformità di Intune utilizza il client DHA (Device Health Attestation) Windows dispositivo. Questo client misura solo lo stato del dispositivo al momento dell'avvio. Pertanto, se un dispositivo non è stato riavviato dopo il completamento della crittografia Bitlocker, il servizio client DHA non segnala Bitlocker come attivo.
 
 