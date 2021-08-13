---
title: Risolvere i problemi relativi alla registrazione di dispositivi Android in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008082"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Risolvere i problemi relativi alla registrazione di dispositivi Android in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema.
  
Alcuni problemi comuni e passaggi di risoluzione:
  
 **Errore dispositivo non crittografato in Portale aziendale:** Le versioni più recenti di Android, in particolare a partire da v7.0, richiedono un passcode di avvio per assicurarsi che il dispositivo sia completamente crittografato. Le soluzioni comuni sono abilitare un pin di avvio o crittografare completamente il dispositivo. Per [ulteriori informazioni,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) vedere questo documento.
  
 **I dispositivi non riescono a eseguire il check-in** con il servizio Intune o vengono visualizzati come "non integri" nella console di amministrazione di Intune: Alcuni dispositivi Samsung 4.4 e 5.5 potrebbero non archiviare il servizio. Esistono 3 possibili soluzioni a questo problema:
  
1. Apri manualmente l'Portale aziendale Intune app, che avvierà automaticamente una sincronizzazione del dispositivo.

2. Aggiorna il dispositivo a Android 6.0 o versione successiva.

3. Disabilitare Samsung Smart Manager dalla gestione della Portale aziendale Intune. Esaminare [questo documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) per ulteriori dettagli su questi problemi e soluzioni.

 **Tipo di licenza utente Errore** non valido o Nome utente non **riconosciuto:** all'utente deve essere assegnata una licenza di Intune o EMS. Esaminare questi documenti per assegnare una licenza tramite: Office'interfaccia di amministrazione o il portale di Azure.
  
Risorse aggiuntive per risolvere il problema:
  
1. Usare [Intune Troubleshooting Portal per](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticare e risolvere gli errori di registrazione comuni. Esaminare [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori dettagli.

2. Esaminare [questo documento](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) per un elenco degli errori comuni che impediscono la registrazione e le risoluzioni per ognuno di essi.

3. [Scopri come registrare i dispositivi Android in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
