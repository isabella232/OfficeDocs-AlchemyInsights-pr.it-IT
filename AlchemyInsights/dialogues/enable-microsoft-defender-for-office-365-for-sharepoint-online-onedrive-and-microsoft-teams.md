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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552424"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Abilitare Microsoft Defender per Office 365 per SharePoint Online, OneDrive e Microsoft Teams

1. Usando le credenziali di amministratore globale o amministratore della sicurezza, accedere al Centro sicurezza [e conformità di Office 365.](https://protection.office.com/)
2. Selezionare **Gestione delle minacce** nel riquadro sinistro, quindi selezionare Allegati **sicuri** del  >  [criterio.](https://protection.office.com/safeattachment)
3. Selezionare **Attiva Microsoft Defender per Office 365 per SharePoint, OneDrive** e Microsoft Teams, quindi selezionare **Salva.**
    > [!TIP]
    >
    > - Come amministratore globale o amministratore di SharePoint Online, eseguire il seguente cmdlet di PowerShell con il parametro **DisallowInfectedFileDownload** impostato su *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Configurare gli avvisi per i file rilevati](https://go.microsoft.com/fwlink/?linkid=2092110)

Per altre informazioni, vedere [Microsoft Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
