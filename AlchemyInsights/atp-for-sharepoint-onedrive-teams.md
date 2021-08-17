---
title: Microsoft Defender per Office 365 per SharePoint, OneDrive, e Microsoft Teams
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
ms.openlocfilehash: 0d0fff3e699d46af2a19a8ad60696b824bafa109
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314966"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender per Office 365 per SharePoint, OneDrive, e Microsoft Teams

Segui questi passaggi per abilitare Microsoft Defender per Office 365:

1. Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account amministratore globale o amministratore della sicurezza.

2. Nel riquadro di spostamento sinistro in **Gestione delle minacce** scegliere Criteri Cassaforte  \> **allegati**.

3. Seleziona **Attiva Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams**.

4. [Creare un criterio di avviso attività](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) per ricevere notifiche quando vengono rilevati file dannosi.

Per le istruzioni complete, vedere Attivare [Cassaforte allegati per SharePoint, OneDrive e Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Nota:** per impostazione predefinita, Microsoft Defender per Office 365 non analizza ogni singolo file in SharePoint Online, OneDrive for Business o Microsoft Teams. I file vengono analizzati in modo asincrono da un processo che usa attività di condivisione, attività guest e segnali di minaccia per identificare i file dannosi. Per ulteriori informazioni, vedere [Cassaforte allegati per SharePoint, OneDrive e Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
