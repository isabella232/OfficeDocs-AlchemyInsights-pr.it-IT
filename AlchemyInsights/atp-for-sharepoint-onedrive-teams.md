---
title: ATP per SharePoint, OneDrive e Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712462"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP per SharePoint, OneDrive e Microsoft Teams

Seguire questa procedura per abilitare Advanced Threat Protection:

1. Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account di amministratore globale o amministratore di sicurezza.

2. Nel riquadro di spostamento a sinistra in **gestione minacce**scegliere **Policy** \> **allegati sicuri**per i criteri.

3. Selezionare **attiva ATP per SharePoint, OneDrive e Microsoft teams**.

4. [Creare un criterio di avviso attività per la](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) ricezione delle notifiche quando vengono rilevati file dannosi.

Per istruzioni complete, vedere questo [argomento](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).

**Nota**: in base alla progettazione, ATP non esegue l'analisi di ogni singolo file in SharePoint Online, OneDrive for business o Microsoft teams. I file vengono analizzati in modo asincrono tramite un processo che utilizza attività di condivisione, attività Guest e segnali di minaccia per identificare i file dannosi. Per ulteriori informazioni, vedere questo [argomento](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
