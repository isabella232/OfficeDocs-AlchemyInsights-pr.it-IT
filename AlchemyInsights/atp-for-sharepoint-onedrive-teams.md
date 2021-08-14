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
ms.openlocfilehash: 9051fb44d7d6bde388d279b3311627848b6f499e30b5eca00d6a47cef105fb77
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997138"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a>Microsoft Defender per Office 365 per SharePoint, OneDrive, e Microsoft Teams

Segui questi passaggi per abilitare Microsoft Defender per Office 365:

1. Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account amministratore globale o amministratore della sicurezza.

2. Nel riquadro di spostamento sinistro in **Gestione delle minacce** scegliere Criteri Cassaforte  \> **allegati.**

3. Seleziona **Attiva Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams**.

4. [Crea un criterio di avviso attività](/microsoft-365/compliance/create-activity-alerts) per ricevere notifiche quando rileviamo file dannosi.

Per istruzioni complete, vedere Attivare [Cassaforte allegati per SharePoint, OneDrive e Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Nota:** per impostazione predefinita, Microsoft Defender per Office 365 non analizza ogni singolo file in SharePoint Online, OneDrive for Business o Microsoft Teams. I file vengono analizzati in modo asincrono da un processo che usa attività di condivisione, attività guest e segnali di minaccia per identificare i file dannosi. Per ulteriori informazioni, vedere [Cassaforte allegati per SharePoint, OneDrive e Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
