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
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543581"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="a748e-102">Microsoft Defender per Office 365 per SharePoint, OneDrive, e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a748e-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="a748e-103">Segui questi passaggi per abilitare Microsoft Defender per Office 365:</span><span class="sxs-lookup"><span data-stu-id="a748e-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="a748e-104">Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account amministratore globale o amministratore della sicurezza.</span><span class="sxs-lookup"><span data-stu-id="a748e-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="a748e-105">Nel riquadro di spostamento sinistro in **Gestione delle minacce** scegliere **Criteri** \> **allegati sicuri.**</span><span class="sxs-lookup"><span data-stu-id="a748e-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="a748e-106">Seleziona **Attiva Defender per Office 365 per SharePoint, OneDrive e Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="a748e-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="a748e-107">[Crea un criterio di avviso attività](/microsoft-365/compliance/create-activity-alerts) per ricevere notifiche quando rileviamo file dannosi.</span><span class="sxs-lookup"><span data-stu-id="a748e-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="a748e-108">Per istruzioni complete, vedere Attivare allegati sicuri per [SharePoint, OneDrive e Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="a748e-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="a748e-109">**Nota:** per impostazione predefinita, Microsoft Defender per Office 365 non analizza ogni singolo file in SharePoint Online, OneDrive for Business o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a748e-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="a748e-110">I file vengono analizzati in modo asincrono da un processo che usa attività di condivisione, attività guest e segnali di minaccia per identificare i file dannosi.</span><span class="sxs-lookup"><span data-stu-id="a748e-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="a748e-111">Per ulteriori informazioni, vedere Allegati sicuri [per SharePoint, OneDrive e Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="a748e-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
