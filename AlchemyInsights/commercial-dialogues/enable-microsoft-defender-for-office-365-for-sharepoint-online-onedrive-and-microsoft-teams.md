---
title: Abilitare Microsoft Defender per Office 365 per SharePoint Online, OneDrive e Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058870"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Abilitare Microsoft Defender per Office 365 per SharePoint Online, OneDrive e Microsoft Teams

1. Usando le credenziali di amministratore globale o amministratore della sicurezza, accedere al Centro sicurezza e conformità Office 365 sicurezza e [conformità.](https://protection.office.com/)
2. Selezionare **Gestione delle minacce** nel riquadro sinistro e quindi selezionare Criteri Cassaforte   >  [allegati](https://protection.office.com/safeattachment).
3. Seleziona **Attiva Microsoft Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams** e quindi seleziona **Salva.**
    > [!TIP]
    >
    > - Come amministratore globale o amministratore di SharePoint Online, eseguire il cmdlet PowerShell seguente con il parametro **DisallowInfectedFileDownload** impostato su *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Configurare gli avvisi per i file rilevati](https://go.microsoft.com/fwlink/?linkid=2092110)

Per altre informazioni, vedi [Microsoft Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
