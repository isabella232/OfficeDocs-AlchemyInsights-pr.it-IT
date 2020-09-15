---
title: Risoluzione dei problemi relativi alla registrazione di dispositivi Android in Microsoft Intune
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689958"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Risoluzione dei problemi relativi alla registrazione di dispositivi Android in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema.
  
Alcuni problemi comuni e passaggi di risoluzione:
  
 **Errore del dispositivo non crittografato nel portale aziendale:** Le versioni più recenti di Android, in particolare a partire da v 7.0, richiedono un codice di accesso all'avvio per assicurarsi che il dispositivo sia completamente crittografato. Le soluzioni comuni sono l'abilitazione di un pin di avvio o la crittografia completa del dispositivo. Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .
  
 I **dispositivi non riescono a eseguire il check-in con il servizio Intune o a essere visualizzati come "non integri" nella console di amministrazione di Intune:** Alcuni dispositivi Samsung 4,4 e 5,5 potrebbero non archiviare il servizio. Esistono tre possibili soluzioni per questo problema:
  
1. Aprire manualmente l'app portale aziendale di Intune, che avvierà automaticamente la sincronizzazione di un dispositivo.

2. Aggiornare il dispositivo a Android 6,0 o versione successiva.

3. Disabilitare Samsung Smart Manager dalla gestione del portale aziendale di Intune. Leggere [questo documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) per ulteriori informazioni su questi problemi e risoluzioni.

 **Tipo di licenza utente non valido** o **nome utente errore non riconosciuto:** all'utente deve essere assegnata una licenza Intune o EMS. Esaminare questi documenti per assegnare una licenza tramite: interfaccia di amministrazione di Office o portale di Azure.
  
Risorse aggiuntive che consentono di risolvere il problema:
  
1. Utilizzare il portale per la [risoluzione dei problemi di Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori di registrazione comuni. Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) .

2. Esaminare [questo documento](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) per un elenco di errori comuni che impediscono la registrazione e le risoluzioni a ciascuno di essi.

3. [Informazioni su come registrare i dispositivi Android in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
