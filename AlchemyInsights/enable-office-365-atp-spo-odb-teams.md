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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543932"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="0c108-102">Abilitare Microsoft Defender per Office 365 per SharePoint Online, OneDrive e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="0c108-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="0c108-103">Andare su https://protection.office.com ed eseguire l'accesso.</span><span class="sxs-lookup"><span data-stu-id="0c108-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="0c108-104">Scegliere **Allegati sicuri per** i  >  **criteri** di gestione  >  **delle minacce**.</span><span class="sxs-lookup"><span data-stu-id="0c108-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="0c108-105">Seleziona **Attiva Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams** e quindi fai clic su **Salva.**</span><span class="sxs-lookup"><span data-stu-id="0c108-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="0c108-106">(Scelta consigliata) Come amministratore globale o amministratore di SharePoint Online, eseguire il cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) con il parametro **DisallowInfectedFileDownload** impostato su *true.*</span><span class="sxs-lookup"><span data-stu-id="0c108-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="0c108-107">(Scelta consigliata) [Configurare gli avvisi](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) per i file rilevati.</span><span class="sxs-lookup"><span data-stu-id="0c108-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="0c108-108">Microsoft Defender per Office 365 non eseguirà l'analisi di ogni singolo file in SharePoint Online, OneDrive o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0c108-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="0c108-109">I file vengono analizzati in modo asincrono, attraverso un processo che usa eventi di condivisione e attività guest, insieme a euristica intelligente e segnali di minaccia per identificare i file dannosi.</span><span class="sxs-lookup"><span data-stu-id="0c108-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="0c108-110">Vedi [Microsoft Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="0c108-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>