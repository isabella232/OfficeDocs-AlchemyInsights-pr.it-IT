---
title: Risoluzione dei problemi con la registrazione di dispositivi Windows Intune Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934780"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Risoluzione dei problemi con la registrazione di dispositivi Windows Intune Microsoft

Esaminare le risorse elencate di seguito per risolvere il problema ora. 
  
Alcuni messaggi di errore comuni e la risoluzione dei passaggi:
  
 **Non è installato il software, 0x80cf4017:** Il certificato per l'account è scaduto. Scaricare nuovamente il pacchetto di software PC Client nella Console di amministrazione Intune. Esaminare la documentazione per ulteriori informazioni. 
  
 **Codice di errore 0x801c0003:** L'errore può verificarsi nei casi seguenti: 
  
1. L'utente dispone di più dispositivi registrati rispetto al limite di dispositivi. Leggere questi documenti per [rimuovere un dispositivo](https://docs.microsoft.com/intune/devices-wipe) o [cambiare il limite di dispositivi](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Gli utenti possono partecipare a dispositivi per Azure Active Directory" è impostato su "none". Impostare su all o selezionare gli utenti. Esaminare la [documentazione](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) per ulteriori informazioni. 
    
3. Il dispositivo è già iscritti da un altro utente. In tal caso, rimuovere il dispositivo dalla console Intune Azure o Annulla manualmente iscrizione del dispositivo prima di tentare nuovamente.
    
4. Il dispositivo è 10 Windows Home Page. Solo Windows 10 Pro, Education Enterprise SKU e possono partecipare alle Azure Active Directory.
    
Risorse aggiuntive per risolvere il problema:
  
1. Utilizzare [Il portale di risoluzione dei problemi Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) per diagnosticare e risolvere gli errori comuni di registrazione. Leggere [questo documento](https://docs.microsoft.com/intune/help-desk-operators) per ulteriori informazioni. 
    
2. Leggere questi documenti per un elenco di errori comuni che impediscono la registrazione e le soluzioni per ognuna: [Guida alla risoluzione dei problemi](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) e [risoluzione dei problemi doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Informazioni su come registrare i dispositivi Windows Intune Microsoft](https://docs.microsoft.com/intune/windows-enroll).
  

