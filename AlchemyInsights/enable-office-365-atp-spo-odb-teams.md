---
title: Abilitazione di Office 365 ATP per SharePoint, OneDrive e Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703430"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="9ffc5-102">Abilitazione di Office 365 Advanced Threat Protection per SharePoint Online, OneDrive e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9ffc5-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="9ffc5-103">Andare su https://protection.office.com ed eseguire l'accesso.</span><span class="sxs-lookup"><span data-stu-id="9ffc5-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="9ffc5-104">Scegliere**allegati sicuri**per i > **criteri** > di **gestione delle minacce**.</span><span class="sxs-lookup"><span data-stu-id="9ffc5-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="9ffc5-105">Selezionare **attiva ATP per SharePoint, OneDrive e Microsoft teams**, quindi fare clic su **Salva**.</span><span class="sxs-lookup"><span data-stu-id="9ffc5-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="9ffc5-106">Consigliato In qualità di amministratore globale o amministratore di SharePoint Online, eseguire il cmdlet [set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) con il parametro **DisallowInfectedFileDownload** impostato su *true*.</span><span class="sxs-lookup"><span data-stu-id="9ffc5-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="9ffc5-107">Consigliato [Configurare gli avvisi](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) per i file rilevati.</span><span class="sxs-lookup"><span data-stu-id="9ffc5-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="9ffc5-108">ATP will nPer analizzare ogni singolo file in SharePoint Online, OneDrive o Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="9ffc5-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="9ffc5-109">I file vengono analizzati in modo asincrono, tramite un processo che utilizza la condivisione e gli eventi di attività Guest, insieme a euristiche intelligenti e ai segnali di minaccia per identificare i file dannosi.</span><span class="sxs-lookup"><span data-stu-id="9ffc5-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="9ffc5-110">Vedere [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="9ffc5-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>