---
title: Risoluzione dei problemi relativi alla registrazione di dispositivi Windows in Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353541"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Risoluzione dei problemi relativi alla registrazione di dispositivi Windows in Microsoft Intune

Esaminare le risorse elencate di seguito per risolvere il problema.
  
Alcuni messaggi di errore comuni e passaggi di risoluzione:
  
 **Non è possibile installare il software, 0x80cf4017:** Il certificato dell'account è scaduto. Scaricare di nuovo il pacchetto software client per PC nella console di amministrazione di Intune. Per ulteriori informazioni, vedere la documentazione seguente.
  
 **Codice di errore 0x801c0003:** È possibile che l'errore si verifichi negli scenari seguenti:
  
1. L'utente dispone di più dispositivi registrati rispetto al limite di dispositivo. Esaminare questi documenti per [rimuovere un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o [modificare il limite del dispositivo](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

2. "Gli utenti possono aggiungere dispositivi ad Azure AD" è impostato su "None". Impostarla su tutti gli utenti o selezionarli. Per ulteriori informazioni, vedere [la documentazione seguente](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

3. Il dispositivo è già registrato da un altro utente. In questo caso, rimuovere il dispositivo dalla console di Azure Intune o annullare la registrazione manuale del dispositivo prima di riprovare.

4. Il dispositivo è Windows 10 Home. Solo gli SKU di Windows 10 Pro, Education e Enterprise sono in grado di partecipare a Azure Active Directory.

Risorse aggiuntive che consentono di risolvere il problema:
  
1. Utilizzare il portale per la [risoluzione dei problemi di Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori di registrazione comuni. Per ulteriori informazioni, vedere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) .

2. Esaminare questi documenti per un elenco di errori comuni che impediscono la registrazione e le risoluzioni a ciascuno di essi: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [risoluzione dei problemi relativi al documento](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Informazioni su come registrare i dispositivi Windows in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
