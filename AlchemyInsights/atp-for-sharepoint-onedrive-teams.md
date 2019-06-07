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
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP per SharePoint, OneDrive e Microsoft Teams

Seguire questa procedura per abilitare Advanced Threat Protection:

1. Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account di amministratore globale o amministratore di sicurezza.

2. Nel riquadro di spostamento a sinistra in **gestione minacce**scegliere **** \> **allegati sicuri**per i criteri.

3. Selezionare **attiva ATP per SharePoint, OneDrive e Microsoft teams**.

4. [Creare un criterio di avviso attività per la](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) ricezione delle notifiche quando vengono rilevati file dannosi.

Per istruzioni complete, vedere questo [argomento](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).

**Nota**: in base alla progettazione, ATP non esegue l'analisi di ogni singolo file in SharePoint Online, OneDrive for business o Microsoft teams. I file vengono analizzati in modo asincrono tramite un processo che utilizza attività di condivisione, attività Guest e segnali di minaccia per identificare i file dannosi. Per ulteriori informazioni, vedere questo [argomento](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
