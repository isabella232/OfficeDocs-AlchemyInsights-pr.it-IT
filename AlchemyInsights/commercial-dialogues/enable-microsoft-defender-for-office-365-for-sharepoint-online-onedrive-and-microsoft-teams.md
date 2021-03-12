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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736368"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Abilitare Microsoft Defender per Office 365 per SharePoint Online, OneDrive e Microsoft Teams

1. Usando le credenziali di amministratore globale o amministratore della sicurezza, accedere al Centro sicurezza e conformità di [Office 365.](https://protection.office.com/)
2. Selezionare **Gestione delle minacce** nel riquadro sinistro e quindi Selezionare **Criteri**  >  [allegati sicuri](https://protection.office.com/safeattachment).
3. Selezionare **Attiva Microsoft Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams** e quindi selezionare **Salva.**
    > [!TIP]
    >
    > - Come amministratore globale o amministratore di SharePoint Online, eseguire il cmdlet PowerShell seguente con il parametro **DisallowInfectedFileDownload** impostato su *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Configurare gli avvisi per i file rilevati](https://go.microsoft.com/fwlink/?linkid=2092110)

Per ulteriori informazioni, vedere [Microsoft Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
