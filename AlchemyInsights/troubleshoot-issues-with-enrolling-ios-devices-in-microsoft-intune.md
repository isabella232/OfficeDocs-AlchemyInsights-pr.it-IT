---
title: Risoluzione dei problemi con la registrazione di dispositivi iOS in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924772"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Risoluzione dei problemi con la registrazione di dispositivi iOS in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema ora. 
  
Alcuni messaggi di errore comuni e la risoluzione dei passaggi:
  
- **Cap dispositivo raggiunto** L'utente dispone di più dispositivi registrati rispetto al limite di dispositivi. Leggere questi documenti per [rimuovere un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o [cambiare il limite di dispositivi](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Questo servizio non è supportato. Nessun criterio di registrazione:** Apple Push Notification Service (APNS) deve essere configurato o rinnovato. Leggere [questo documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) per istruzioni su come effettuare tale operazione. 
    
- **Tipo di licenza utente non valido o il nome utente non riconosciuto:** L'utente deve essere assegnato una licenza Intune o EMS. Leggere questi documenti per assegnare una licenza tramite: [Interfaccia di amministrazione di Office](https://docs.microsoft.com/intune/licenses-assign) o [portale Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Risorse aggiuntive per risolvere il problema:
  
1. Utilizzare [Il portale di risoluzione dei problemi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori comuni di registrazione. Leggere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori informazioni. 
    
2. Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le soluzioni per ognuna: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [risoluzione dei problemi doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Informazioni su come registrare dispositivi iOS in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

