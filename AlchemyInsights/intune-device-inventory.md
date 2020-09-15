---
title: Inventario dispositivi Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667882"
---
# <a name="intune-device-inventory"></a>Inventario dispositivi Intune

Il pannello Dispositivi fornisce all'amministratore informazioni dettagliate sui dispositivi gestiti in Intune per ogni dispositivo. Le informazioni visualizzate includono: hardware, applicazioni individuate, stato di conformità e stato di configurazione del dispositivo.

I dati di inventario per l'hardware e le applicazioni individuate vengono raccolti ogni sette giorni. Le applicazioni e gli elementi specifici dell'hardware segnalato variano in base al sistema operativo del dispositivo e al fatto che il dispositivo sia di proprietà personale o aziendale.

Per altre informazioni, consultare [Vedere i dettagli del dispositivo in Intune](https://docs.microsoft.com/intune/device-inventory).

**Domande frequenti**

D: non ricevo un elenco completo delle applicazioni presenti nei dispositivi Windows registrati in Intune. Perché?

R: al momento, compaiono nell'elenco solo le app moderne per PC Windows 10 identificati come dispositivi aziendali. Intune non raccoglie informazioni sulle app Win32 installate su questi dispositivi.

D: perché i numeri di telefono non vengono raccolti da tutti i dispositivi?

R: i telefoni categorizzati come dispositivi aziendali in Intune non vengono identificati con il numero di telefono completo quando, ad esempio, si esegue un report inventario di dispositivi mobili. I numeri di telefono Bring-You-Own-Device sono sempre parzialmente mascherati da asterischi (****) e mostrano solo le ultime quattro cifre.