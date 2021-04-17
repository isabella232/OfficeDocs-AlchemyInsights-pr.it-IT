---
title: Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823467"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema. 
  
Alcuni messaggi di errore comuni e passaggi di risoluzione:
  
- **Raggiunto il limite massimo del dispositivo** L'utente ha registrato più dispositivi rispetto al limite del dispositivo. Esaminare questi documenti per [rimuovere un dispositivo o](https://docs.microsoft.com/intune/devices-wipe) modificare il limite del [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Questo servizio non è supportato. Nessun criterio di registrazione:** apple push notification service (APNS) deve essere configurato o rinnovato. Leggere [questo documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) per istruzioni su come eseguire questa operazione. 
    
- **Tipo di licenza utente Non valido o Nome utente non riconosciuto:** All'utente deve essere assegnata una licenza di Intune o EMS. Esaminare questi documenti per assegnare una licenza tramite: [Interfaccia di amministrazione di Office](https://docs.microsoft.com/intune/licenses-assign) o portale di [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Risorse aggiuntive per risolvere il problema:
  
1. Usare [Intune Troubleshooting Portal per](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticare e risolvere gli errori di registrazione comuni. Esaminare [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori dettagli. 
    
2. Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [Documento di risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Scopri come registrare i dispositivi iOS in Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

