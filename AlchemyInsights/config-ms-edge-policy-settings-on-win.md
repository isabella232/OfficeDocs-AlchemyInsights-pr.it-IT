---
title: Configurare le impostazioni del criterio Microsoft Edge in Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576475"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="8ac6a-102">Configurare le impostazioni del criterio Microsoft Edge in Windows</span><span class="sxs-lookup"><span data-stu-id="8ac6a-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="8ac6a-103">Per configurare le impostazioni dei criteri e gli aggiornamenti gestiti per Microsoft Edge, utilizzare oggetti Criteri di gruppo (GPO).</span><span class="sxs-lookup"><span data-stu-id="8ac6a-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="8ac6a-104">È inoltre possibile eseguire il provisioning dei criteri tramite il registro di sistema. Questo sarebbe appropriato per (1) dispositivi di Windows aggiunti a un dominio Microsoft Active Directory e per (2) Windows 10 Pro e le istanze Enterprise per la gestione dei dispositivi in Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="8ac6a-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="8ac6a-105">Per configurare Microsoft Edge tramite GPO, eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="8ac6a-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="8ac6a-106">All'archivio centrale criteri di gruppo nel dominio di Active Directory o alla cartella del modello di definizione dei criteri nei singoli computer, installare tutti i modelli amministrativi che aggiungono regole e impostazioni per Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="8ac6a-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="8ac6a-107">Configurare i criteri specifici che si desidera impostare.</span><span class="sxs-lookup"><span data-stu-id="8ac6a-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="8ac6a-108">Per ulteriori informazioni, vedere [Configure Microsoft Edge Policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="8ac6a-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
