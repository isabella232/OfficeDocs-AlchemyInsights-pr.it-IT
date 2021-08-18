---
title: Abilitare Office 365 ATP per SharePoint, OneDrive e Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4a29fdf1b61dd51b85793a1346bea193c67f70d32344470cb5449cf767da4a24
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896607"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Abilitare Microsoft Defender per Office 365 per SharePoint Online, OneDrive e Microsoft Teams

1. Andare su https://protection.office.com ed eseguire l'accesso.
2. Scegliere **Criteri di gestione**  >  **delle** minacce Cassaforte  >  **allegati**.
3. Seleziona **Attiva Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams** e quindi fai clic su **Salva.**
4. (Scelta consigliata) Come amministratore globale o amministratore di SharePoint Online, eseguire il cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) con il parametro **DisallowInfectedFileDownload** impostato su *true.*
5. (Scelta consigliata) [Configurare gli avvisi](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) per i file rilevati.

> [!NOTE]
> Microsoft Defender per Office 365 non eseguirà l'analisi di ogni singolo file in SharePoint Online, OneDrive o Microsoft Teams. I file vengono analizzati in modo asincrono, attraverso un processo che usa eventi di condivisione e attività guest, insieme a euristica intelligente e segnali di minaccia per identificare i file dannosi. Vedi [Microsoft Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).