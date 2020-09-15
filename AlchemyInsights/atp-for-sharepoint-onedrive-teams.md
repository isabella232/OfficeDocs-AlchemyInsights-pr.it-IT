---
title: ATP per SharePoint, OneDrive e Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715565"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP per SharePoint, OneDrive e Microsoft Teams

Seguire questa procedura per abilitare Advanced Threat Protection:

1. Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account di amministratore globale o amministratore di sicurezza.

2. Nel riquadro di spostamento a sinistra in **gestione minacce**scegliere **Policy** \> **allegati sicuri**per i criteri.

3. Selezionare **attiva ATP per SharePoint, OneDrive e Microsoft teams**.

4. [Creare un criterio di avviso attività per la](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) ricezione delle notifiche quando vengono rilevati file dannosi.

Per istruzioni complete, vedere questo [argomento](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Nota**: in base alla progettazione, ATP non esegue l'analisi di ogni singolo file in SharePoint Online, OneDrive for business o Microsoft teams. I file vengono analizzati in modo asincrono tramite un processo che utilizza attività di condivisione, attività Guest e segnali di minaccia per identificare i file dannosi. Per ulteriori informazioni, vedere questo [argomento](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
