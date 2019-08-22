---
title: Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507007"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Risolvere i problemi relativi alla registrazione dei dispositivi iOS in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema. 
  
Alcuni messaggi di errore comuni e passaggi di risoluzione:
  
- **Tappo del dispositivo raggiunto** L'utente dispone di più dispositivi registrati rispetto al limite di dispositivo. Esaminare questi documenti per [rimuovere un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o [modificare il limite del dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Questo servizio non è supportato. Nessun criterio di registrazione:** è necessario configurare o rinnovare il servizio di notifica push di Apple (APNS). Leggere [questo documento](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) per istruzioni su come eseguire questa operazione. 
    
- **Tipo di licenza utente non valido o nome utente non riconosciuto:** All'utente deve essere assegnata una licenza Intune o EMS. Esaminare questi documenti per assegnare una licenza tramite: interfaccia di [amministrazione di Office](https://docs.microsoft.com/intune/licenses-assign) o [portale di Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Risorse aggiuntive che consentono di risolvere il problema:
  
1. Utilizzare il portale per la [risoluzione dei problemi di Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori di registrazione comuni. Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Esaminare questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni a ciascuno di essi: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) e [risoluzione dei problemi relativi al documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Informazioni su come registrare i dispositivi iOS in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

