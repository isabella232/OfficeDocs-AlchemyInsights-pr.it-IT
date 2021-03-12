---
title: Risolvere i problemi relativi alla registrazione dei dispositivi Windows in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708894"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Risolvere i problemi relativi alla registrazione dei dispositivi Windows in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema.
  
Alcuni messaggi di errore comuni e procedure di risoluzione:
  
 **Il software non può essere installato, 0x80cf4017:** Il certificato dell'account è scaduto. Scaricare di nuovo il pacchetto software del client PC nella console di amministrazione di Intune. Per ulteriori informazioni, vedere questa documentazione.
  
 **Codice di errore 0x801c0003:** L'errore può verificarsi negli scenari seguenti:
  
-  L'utente ha più dispositivi registrati rispetto al limite di dispositivi. Esaminare questi documenti per [rimuovere un dispositivo o](https://docs.microsoft.com/intune/devices-wipe) modificare il limite del [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Gli utenti possono aggiungere dispositivi ad Azure AD" è impostato su "nessuno". Impostarla su tutti gli utenti o selezionarli. Per [ulteriori informazioni, consultare](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) questa documentazione.

-  Il dispositivo è già registrato da un altro utente. In questo caso, rimuovere il dispositivo dalla console di Azure Intune o annullare manualmente la registrazione del dispositivo prima di riprovare.

-  Il dispositivo è Windows 10 Home. Solo le SKU Windows 10 Pro, Education ed Enterprise possono aggiungersi ad Azure Active Directory.

Risorse aggiuntive per risolvere il problema:
  
-  Usare [il portale per la risoluzione dei](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) problemi di Intune per diagnosticare e risolvere gli errori di registrazione comuni. Per [ulteriori dettagli,](https://docs.microsoft.com/intune/help-desk-operators) consultare questo documento.

-  Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [Documento di risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Informazioni su come registrare i dispositivi Windows in Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
