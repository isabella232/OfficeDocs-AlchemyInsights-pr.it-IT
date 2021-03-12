---
title: Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708966"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema. 
  
Alcuni messaggi di errore comuni e procedure di risoluzione:
  
- **Limite massimo dispositivo raggiunto** L'utente ha più dispositivi registrati rispetto al limite di dispositivi. Esaminare questi documenti per [rimuovere un dispositivo o](https://docs.microsoft.com/intune/devices-wipe) modificare il limite del [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Questo servizio non è supportato. Nessun criterio di registrazione:** il servizio apns (Apple Push Notification Service) deve essere configurato o rinnovato. Leggere [questo documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) per istruzioni su come eseguire questa operazione. 
    
- **Tipo di licenza utente non valido o Nome utente non riconosciuto:** All'utente deve essere assegnata una licenza di Intune o EMS. Rivedere questi documenti per assegnare una licenza tramite [l'interfaccia di amministrazione di Office](https://docs.microsoft.com/intune/licenses-assign) o il portale di [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Risorse aggiuntive per risolvere il problema:
  
1. Usare [il portale per la risoluzione dei](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) problemi di Intune per diagnosticare e risolvere gli errori di registrazione comuni. Per [ulteriori dettagli,](https://docs.microsoft.com/intune/help-desk-operators) consultare questo documento. 
    
2. Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [Documento di risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Informazioni su come registrare i dispositivi iOS in Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

