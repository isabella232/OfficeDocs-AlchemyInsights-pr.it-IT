---
title: Dispositivi di Configuration Manager mancanti nel portale
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: b6538cb6a348e194856024680a25af948152910a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812155"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="b4644-102">Dispositivi di Configuration Manager mancanti nel portale</span><span class="sxs-lookup"><span data-stu-id="b4644-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="b4644-103">Per il funzionamento della sincronizzazione dei dispositivi, gli [endpoint Internet necessari](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) devono essere raggiungibili dal server locale che ospita il ruolo del punto di connessione del servizio.</span><span class="sxs-lookup"><span data-stu-id="b4644-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="b4644-104">Per risolvere i problemi di sincronizzazione dei dispositivi, consultare il file **CMGatewaySyncUploadWorker.log** disponibile nel punto di connessione del servizio.</span><span class="sxs-lookup"><span data-stu-id="b4644-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="b4644-105">Per altre informazioni, vedere [Collegamento di tenant in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="b4644-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
