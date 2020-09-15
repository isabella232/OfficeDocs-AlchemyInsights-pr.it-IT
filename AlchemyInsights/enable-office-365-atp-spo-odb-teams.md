---
title: Abilitazione di Office 365 ATP per SharePoint, OneDrive e Microsoft Teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709911"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Abilitazione di Office 365 Advanced Threat Protection per SharePoint Online, OneDrive e Microsoft Teams

1. Andare su https://protection.office.com ed eseguire l'accesso.
2. Scegliere **Threat management**  >  **Policy**  >  **allegati sicuri**per i criteri di gestione delle minacce.
3. Selezionare **attiva ATP per SharePoint, OneDrive e Microsoft teams**, quindi fare clic su **Salva**.
4. Consigliato In qualità di amministratore globale o amministratore di SharePoint Online, eseguire il cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) con il parametro **DisallowInfectedFileDownload** impostato su *true*.
5. Consigliato [Configurare gli avvisi](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) per i file rilevati.

> [!NOTE]
> ATP will nPer analizzare ogni singolo file in SharePoint Online, OneDrive o Microsoft teams. I file vengono analizzati in modo asincrono, tramite un processo che utilizza la condivisione e gli eventi di attività Guest, insieme a euristiche intelligenti e ai segnali di minaccia per identificare i file dannosi. Vedere [ATP per SharePoint, OneDrive e Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).