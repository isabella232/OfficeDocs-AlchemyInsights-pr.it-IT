---
title: Problemi con la rimozione di un dispositivo disattivato o rimosso dall'inventario dei dispositivi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 814301e9cd8197e62dcca68ab3bdde1618d210f73a744b53bb5af7b861eb02bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54076656"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Problemi con la rimozione di un dispositivo disattivato o rimosso dall'inventario dei dispositivi

Microsoft Defender for Endpoint attualmente non consente la rimozione manuale del record del dispositivo di un dispositivo offboarding o rimosso dall'inventario dei dispositivi.

Per motivi di sicurezza, il dispositivo rimane nel portale come record cronologico fino a 180 giorni. Tuttavia, i dati del dispositivo vengono eliminati in base al periodo di conservazione configurato.

**Nota:** Un dispositivo disattivato o disattivato passa automaticamente allo stato **Inattivo** dopo sette giorni. Inoltre, i dispositivi non attivi negli ultimi 30 giorni non vengono fattoriati nei dati che riflettono il punteggio di esposizione dell'organizzazione gestione di minacce e vulnerabilità o Microsoft Secure Score per i dispositivi.
 
Se ancora non vuoi visualizzare determinati dispositivi nella visualizzazione Inventario dispositivi, prova a inserire un tag del dispositivo per filtrare il dispositivo rimosso dalla visualizzazione Inventario dispositivi.

Per altre informazioni, vedere:

[Dispositivi offboard dal servizio Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Punteggio di esposizione in gestione di minacce e vulnerabilità](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Risolvere i sensori non integri in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Come usare il tagging in modo efficace (parte 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Come usare il tagging in modo efficace (parte 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Come usare il tagging in modo efficace (parte 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




