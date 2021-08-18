---
title: Microsoft Edge configurare le impostazioni di privacy
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114176"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge configurare le impostazioni di privacy

Per impostazione predefinita, se Microsoft Edge viene distribuito su piattaforme non Windows, i dati di diagnostica e le informazioni sul sito non vengono inviati a Microsoft. Tuttavia, se Microsoft Edge vengono distribuiti in Windows 10, i dati di diagnostica e le informazioni del sito vengono inviati in base alle impostazioni dei dati di diagnostica Windows [degli utenti.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Per configurare il modo Microsoft Edge gestire la raccolta dati per l'organizzazione, utilizzare i criteri di gruppo seguenti:
- [MetricsReportingEnabled:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)questo criterio consente la segnalazione dei dati relativi all'utilizzo e agli arresti anomalo.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)questo criterio invia informazioni sul sito utilizzate per migliorare la servizi Microsoft.

Per ulteriori informazioni, vedere [Configure policy settings.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)