---
title: Risolvere i problemi relativi alla registrazione dei dispositivi Android in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709002"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Risolvere i problemi relativi alla registrazione dei dispositivi Android in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema.
  
Alcuni problemi comuni e procedure di risoluzione:
  
 **Errore dispositivo non crittografato nel portale aziendale:** Le versioni più recenti di Android, in particolare a partire dalla versione 7.0, richiedono un passcode di avvio per assicurarsi che il dispositivo sia completamente crittografato. Le soluzioni comuni sono abilitare un pin di avvio o crittografare completamente il dispositivo. Per [ulteriori informazioni,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) consultare questo documento.
  
 **I dispositivi non riescono a eseguire l'archiviazione** con il servizio Intune o a visualizzare "Non integro" nella console di amministrazione di Intune: Alcuni dispositivi Samsung 4.4 e 5.5 potrebbero non archiviare il servizio. Esistono 3 possibili soluzioni a questo problema:
  
1. Apri manualmente l'app Portale aziendale intune, che avvierà automaticamente la sincronizzazione del dispositivo.

2. Aggiorna il dispositivo a Android 6.0 o versione successiva.

3. Disabilitare La gestione del portale aziendale di Intune da parte di Samsung Smart Manager. Leggere [questo documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) per ulteriori dettagli su questi problemi e soluzioni.

 **User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Esaminare questi documenti per assegnare una licenza tramite l'interfaccia di amministrazione di Office o il portale di Azure.
  
Risorse aggiuntive per risolvere il problema:
  
1. Usare [il portale per la risoluzione dei](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) problemi di Intune per diagnosticare e risolvere gli errori di registrazione comuni. Per [ulteriori dettagli,](https://docs.microsoft.com/intune/help-desk-operators) consultare questo documento.

2. Esaminare [questo documento per](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) un elenco degli errori comuni che impediscono la registrazione e le risoluzioni per ognuno di essi.

3. [Informazioni su come registrare i dispositivi Android in Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
