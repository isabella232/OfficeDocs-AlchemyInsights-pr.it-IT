---
title: Risoluzione dei problemi con la registrazione di dispositivi Android Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475796"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Risoluzione dei problemi con la registrazione di dispositivi Android Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema ora.
  
Alcuni problemi comuni e la risoluzione dei passaggi:
  
 **Dispositivo non crittografate errore nel portale aziendale:** Versioni più recenti di Android, in particolare a partire da v 7.0, richiedono un passcode di avvio per verificare che il dispositivo è completamente crittografato. Per attivare un pin avvio o completamente crittografare il dispositivo sono soluzioni comuni. Leggere [questo documento](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) per ulteriori informazioni. 
  
 **Riusciranno a verificare con il servizio Intune o visualizzato come "Problematica" la console di amministrazione Intune:** Alcuni 4.4 Samsung e 5.5 dispositivi non possono controllare nel servizio. Sono disponibili 3 possibili soluzioni a questo problema: 
  
1. Aprire manualmente app Intune portale della società, che verrà avviata automaticamente la sincronizzazione del dispositivo.
    
2. Aggiornare il dispositivo a Android 6.0 o versioni successive.
    
3. Disabilitare Samsung Smart Manager di gestione del portale aziendale Intune. Leggere [questo documento](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) per ulteriori informazioni su questi problemi e soluzioni. 
    
 **Utente licenza tipo valido** o **nome utente non riconosciuto errore:** è necessario assegnare una licenza Intune o em. Leggere questi documenti per assegnare una licenza a: portale di interfaccia di amministrazione di Office o Azure. 
  
Risorse aggiuntive per risolvere il problema:
  
1. Utilizzare [Il portale di risoluzione dei problemi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori comuni di registrazione. Leggere [questo documento](https://docs.microsoft.com/en-us/intune/help-desk-operators) per ulteriori informazioni. 
    
2. Leggere [questo documento](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) per un elenco di errori comuni che impediscono la registrazione e le soluzioni per ognuno. 
    
3. [Informazioni su come registrare dispositivi Android Intune Microsoft](https://docs.microsoft.com/en-us/intune/android-enroll).
    

