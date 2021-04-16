---
title: Risolvere i problemi relativi alla registrazione di dispositivi Windows in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808975"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Risolvere i problemi relativi alla registrazione di dispositivi Windows in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema.
  
Alcuni messaggi di errore comuni e passaggi di risoluzione:
  
 **Il software non può essere installato, 0x80cf4017:** Il certificato dell'account è scaduto. Scaricare di nuovo il pacchetto software pc client nella Console di amministrazione di Intune. Per ulteriori informazioni, vedere questa documentazione.
  
 **Codice di errore 0x801c0003:** L'errore può verificarsi negli scenari seguenti:
  
-  L'utente ha registrato più dispositivi rispetto al limite del dispositivo. Esaminare questi documenti per [rimuovere un dispositivo o](https://docs.microsoft.com/intune/devices-wipe) modificare il limite del [dispositivo.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Gli utenti possono aggiungere dispositivi ad Azure AD" è impostato su "nessuno". Impostarlo su tutti gli utenti o selezionarli. Per [ulteriori informazioni, vedere](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) questa documentazione.

-  Il dispositivo è già registrato da un altro utente. In questo caso, rimuovere il dispositivo dalla console di Azure Intune o annullare manualmente la registrazione del dispositivo prima di riprovare.

-  Il dispositivo è Windows 10 Home. Solo gli SKU Di Windows 10 Pro, Education ed Enterprise possono partecipare ad Azure Active Directory.

Risorse aggiuntive per risolvere il problema:
  
-  Usare [Intune Troubleshooting Portal per](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticare e risolvere gli errori di registrazione comuni. Esaminare [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori dettagli.

-  Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [Documento di risoluzione dei problemi](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Scopri come registrare i dispositivi Windows in Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
