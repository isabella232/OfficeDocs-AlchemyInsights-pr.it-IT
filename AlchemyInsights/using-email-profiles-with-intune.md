---
title: Utilizzo dei profili di posta elettronica con Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505216"
---
# <a name="using-email-profiles-with-intune"></a>Utilizzo dei profili di posta elettronica con Intune

Intune può essere usato per creare e distribuire profili di posta elettronica per il client di posta elettronica nativo (predefinito) su più piattaforme di dispositivi.

Per informazioni su alcune delle restrizioni associate ai profili di posta elettronica, incluse informazioni su come è gestita la presenza dei profili esistenti e come rimuovere i profili di posta elettronica, si veda [Aggiungere le impostazioni di posta elettronica ai dispositivi con Intune](https://docs.microsoft.com/intune/email-settings-configure).

Per altre informazioni su come creare profili di posta elettronica per ogni piattaforma del dispositivo, si veda:

[Impostazioni dei dispositivi Android per configurare la posta elettronica, l'autenticazione e la sincronizzazione in Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Aggiungere impostazioni di posta elettronica per i dispositivi iOS e iPadOS in Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Impostazioni del profilo di posta elettronica in Microsoft Intune per dispositivi che utilizzano Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Impostazioni del profilo di posta elettronica per i dispositivi che utilizzano Windows 10 in Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Problema di sincronizzazione comune**

**Il profilo di posta elettronica Knox su Android impedisce che i contatti, il calendario e le attività degli utenti siano sincronizzati con i dispositivi degli utenti.**

Il profilo di posta elettronica Knox su Android offre agli amministratori la possibilità di decidere quali tipi di contenuto vengano sincronizzati con il dispositivo, configurando ogni tipo di contenuto in modo che sia abilitato.

Se l'impostazione di uno dei tipi di contenuto è impostata su **Non configurato** (impostazione predefinita), quel tipo di contenuto non viene sincronizzato automaticamente. Un utente può abilitare manualmente il tipo di contenuto che vuole sincronizzare direttamente nel dispositivo, ma tale configurazione viene sovrascritta dall'impostazione dei criteri di Intune e la sincronizzazione si interrompe per quel tipo di contenuto.

