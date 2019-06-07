---
title: ATP per SharePoint, OneDrive e Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765168"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="852ec-102">ATP per SharePoint, OneDrive e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="852ec-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="852ec-103">Seguire questa procedura per abilitare Advanced Threat Protection:</span><span class="sxs-lookup"><span data-stu-id="852ec-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="852ec-104">Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account di amministratore globale o amministratore di sicurezza.</span><span class="sxs-lookup"><span data-stu-id="852ec-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="852ec-105">Nel riquadro di spostamento a sinistra in **gestione minacce**scegliere \*\*\*\* \> **allegati sicuri**per i criteri.</span><span class="sxs-lookup"><span data-stu-id="852ec-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="852ec-106">Selezionare **attiva ATP per SharePoint, OneDrive e Microsoft teams**.</span><span class="sxs-lookup"><span data-stu-id="852ec-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="852ec-107">[Creare un criterio di avviso attività per la](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) ricezione delle notifiche quando vengono rilevati file dannosi.</span><span class="sxs-lookup"><span data-stu-id="852ec-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="852ec-108">Per istruzioni complete, vedere questo [argomento](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="852ec-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="852ec-109">**Nota**: in base alla progettazione, ATP non esegue l'analisi di ogni singolo file in SharePoint Online, OneDrive for business o Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="852ec-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="852ec-110">I file vengono analizzati in modo asincrono tramite un processo che utilizza attività di condivisione, attività Guest e segnali di minaccia per identificare i file dannosi.</span><span class="sxs-lookup"><span data-stu-id="852ec-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="852ec-111">Per ulteriori informazioni, vedere questo [argomento](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="852ec-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
