---
title: Configurare le impostazioni di privacy in Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 991f323249e15abd137c3e69b400e40503ed30dec6507cc5071a0b1af7f72bb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090308"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Configurare le impostazioni di privacy in Microsoft Edge

Per impostazione predefinita, se Microsoft Edge viene distribuito su piattaforme non Windows, i dati di diagnostica e le informazioni sul sito non vengono inviati a Microsoft. Tuttavia, se Microsoft Edge vengono distribuiti in Windows 10, i dati di diagnostica e le informazioni del sito vengono inviati in base alle impostazioni dei dati di diagnostica Windows [degli utenti.](https://go.microsoft.com/fwlink/?linkid=2132472)

Per configurare il modo Microsoft Edge gestire la raccolta dati per l'organizzazione, utilizzare i criteri di gruppo seguenti:
- [MetricsReportingEnabled attiva](https://go.microsoft.com/fwlink/?linkid=2132470) la segnalazione dei dati relativi all'utilizzo e agli arresti anomalo.
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) invia informazioni sul sito utilizzate per migliorare la servizi Microsoft.

Per ulteriori informazioni, vedere [Configure policy settings.](https://go.microsoft.com/fwlink/?linkid=2132577)
