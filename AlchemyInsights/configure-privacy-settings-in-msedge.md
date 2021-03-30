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
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403861"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="a5339-102">Configurare le impostazioni di privacy in Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a5339-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="a5339-103">Per impostazione predefinita, se Microsoft Edge viene distribuito su piattaforme non Windows, i dati di diagnostica e le informazioni sul sito non vengono inviati a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a5339-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="a5339-104">Tuttavia, se Microsoft Edge è distribuito in Windows 10, i dati di diagnostica e le informazioni del sito vengono inviati in base alle impostazioni dei dati di [diagnostica di Windows degli utenti.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="a5339-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="a5339-105">Per configurare il modo in cui Microsoft Edge gestisce la raccolta dei dati per l'organizzazione, utilizzare i criteri di gruppo seguenti:</span><span class="sxs-lookup"><span data-stu-id="a5339-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="a5339-106">[MetricsReportingEnabled attiva](https://go.microsoft.com/fwlink/?linkid=2132470) la segnalazione dei dati relativi all'utilizzo e agli arresti anomalo.</span><span class="sxs-lookup"><span data-stu-id="a5339-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="a5339-107">[SendSiteInfoToImproveServices invia](https://go.microsoft.com/fwlink/?linkid=2132470) informazioni sul sito utilizzate per migliorare i servizi Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a5339-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="a5339-108">Per ulteriori informazioni, vedere [Configure policy settings.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="a5339-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
