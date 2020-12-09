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
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="3cc4c-102">Microsoft Edge configurare le impostazioni di privacy</span><span class="sxs-lookup"><span data-stu-id="3cc4c-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="3cc4c-103">Per impostazione predefinita, se Microsoft Edge è distribuito su piattaforme non Windows, i dati di diagnostica e le informazioni sui siti non vengono inviati a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3cc4c-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="3cc4c-104">Tuttavia, se Microsoft Edge è distribuito in Windows 10, i dati di diagnostica e le informazioni sul sito vengono inviati in base alle [impostazioni dei dati di diagnostica di Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)degli utenti.</span><span class="sxs-lookup"><span data-stu-id="3cc4c-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="3cc4c-105">Per configurare il modo in cui Microsoft Edge gestisce la raccolta dei dati per l'organizzazione, utilizzare i seguenti criteri di gruppo:</span><span class="sxs-lookup"><span data-stu-id="3cc4c-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="3cc4c-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): questo criterio consente di segnalare i dati relativi all'utilizzo e ai crash.</span><span class="sxs-lookup"><span data-stu-id="3cc4c-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="3cc4c-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): questo criterio consente di inviare le informazioni del sito utilizzate per migliorare i servizi Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3cc4c-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="3cc4c-108">Per ulteriori informazioni, vedere [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="3cc4c-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>