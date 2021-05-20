---
title: Risoluzione dei problemi di Microsoft Defender per Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545272"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="d87df-102">Risoluzione dei problemi di Microsoft Defender per Office 365</span><span class="sxs-lookup"><span data-stu-id="d87df-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="d87df-103">**Si nota un ritardo nel recapito dei messaggi?**</span><span class="sxs-lookup"><span data-stu-id="d87df-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="d87df-104">Usa [l'opzione Recapito](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) dinamico in Microsoft Defender per Office 365 allegati sicuri.</span><span class="sxs-lookup"><span data-stu-id="d87df-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="d87df-105">Ciò consente di evitare ritardi nei messaggi proteggendo i destinatari da file dannosi.</span><span class="sxs-lookup"><span data-stu-id="d87df-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="d87df-106">**Si desidera segnalare falsi positivi o falsi negativi a Microsoft?**</span><span class="sxs-lookup"><span data-stu-id="d87df-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="d87df-107">Usa [Esplora invii](https://protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="d87df-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="d87df-108">-\*\* Si è verificato che è possibile abilitare la protezione dei collegamenti sicuri per la posta elettronica interna inviata tra destinatari all'interno dell'organizzazione?\*\* Eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="d87df-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="d87df-109">Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account amministratore globale o amministratore della sicurezza.</span><span class="sxs-lookup"><span data-stu-id="d87df-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="d87df-110">Nel riquadro di spostamento a sinistra in **Gestione delle minacce** scegliere Collegamenti **sicuri** per i \> **criteri.**</span><span class="sxs-lookup"><span data-stu-id="d87df-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="d87df-111">Nella sezione **Criteri applicabili all'intera organizzazione** selezionare il criterio e fare clic su **Modifica.**</span><span class="sxs-lookup"><span data-stu-id="d87df-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="d87df-112">In **Impostazioni**, abilitare **Applica collegamenti sicuri ai messaggi inviati all'interno dell'organizzazione**.</span><span class="sxs-lookup"><span data-stu-id="d87df-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
