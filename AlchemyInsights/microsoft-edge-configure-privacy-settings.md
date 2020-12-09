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
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599514"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge configurare le impostazioni di privacy

Per impostazione predefinita, se Microsoft Edge è distribuito su piattaforme non Windows, i dati di diagnostica e le informazioni sui siti non vengono inviati a Microsoft. Tuttavia, se Microsoft Edge è distribuito in Windows 10, i dati di diagnostica e le informazioni sul sito vengono inviati in base alle [impostazioni dei dati di diagnostica di Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)degli utenti.

Per configurare il modo in cui Microsoft Edge gestisce la raccolta dei dati per l'organizzazione, utilizzare i seguenti criteri di gruppo:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): questo criterio consente di segnalare i dati relativi all'utilizzo e ai crash.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): questo criterio consente di inviare le informazioni del sito utilizzate per migliorare i servizi Microsoft.

Per ulteriori informazioni, vedere [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).