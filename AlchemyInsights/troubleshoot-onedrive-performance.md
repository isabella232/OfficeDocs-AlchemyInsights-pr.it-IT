---
title: Risoluzione dei problemi relativi alle prestazioni di OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 222f818c3fd78a19b9952d4703755498bc080910
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822202"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="2dd8e-102">Risoluzione dei problemi relativi alle prestazioni di OneDrive</span><span class="sxs-lookup"><span data-stu-id="2dd8e-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="2dd8e-103">Se si verifica una sincronizzazione più lenta del previsto o problemi di prestazioni simili con OneDrive:</span><span class="sxs-lookup"><span data-stu-id="2dd8e-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="2dd8e-104">Verificare che non siano presenti problemi noti con il [dashboard di integrità dei servizi](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="2dd8e-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="2dd8e-105">[Abilitare i file su richiesta](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) in modo che sia possibile accedere a tutti i file in OneDrive senza doverli scaricare tutti e utilizzare lo spazio di archiviazione nel dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2dd8e-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="2dd8e-106">[Esaminare le procedure consigliate](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) per la pianificazione e le prestazioni di rete.</span><span class="sxs-lookup"><span data-stu-id="2dd8e-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="2dd8e-107">[Massimizzare la velocità di caricamento e download](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), soprattutto se si sta sincronizzando un dispositivo per la prima volta.</span><span class="sxs-lookup"><span data-stu-id="2dd8e-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="2dd8e-108">Se si sta sincronizzando una raccolta con più di 100.000 elementi, la sincronizzazione di OneDrive può sembrare bloccata per un lungo periodo di tempo oppure lo stato Visualizza l'elaborazione di 0KB di xMB.</span><span class="sxs-lookup"><span data-stu-id="2dd8e-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="2dd8e-109">Ulteriori [informazioni sulla sincronizzazione di più di 100.000 file](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) e il [limite supportato di OneDrive per i file 300.000](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="2dd8e-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="2dd8e-110">Quando un utente supera i limiti di utilizzo, in SharePoint Online vengono strozzate eventuali ulteriori richieste provenienti da tale account utente per un breve periodo.</span><span class="sxs-lookup"><span data-stu-id="2dd8e-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="2dd8e-111">Tutte le azioni dell'utente vengono limitate quando la limitazione è attiva.</span><span class="sxs-lookup"><span data-stu-id="2dd8e-111">All user actions are throttled while the throttle is in effect.</span></span>
