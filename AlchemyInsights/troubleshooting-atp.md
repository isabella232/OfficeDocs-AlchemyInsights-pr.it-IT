---
title: Risoluzione dei problemi relativi a Office 365 Advanced Threat Protection
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: c90c8e9cb23cba93883cc1148fcbca77c9e92408
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732406"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="a7f6b-102">Risoluzione dei problemi relativi a Office 365 Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="a7f6b-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="a7f6b-103">Si notano ritardi nel recapito del messaggio?</span><span class="sxs-lookup"><span data-stu-id="a7f6b-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="a7f6b-104">Utilizzare l'opzione per il [recapito dinamico](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) nel criterio degli allegati sicuri di ATP.</span><span class="sxs-lookup"><span data-stu-id="a7f6b-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="a7f6b-105">In questo modo si eviteranno ritardi nei messaggi proteggendo i destinatari da file dannosi.</span><span class="sxs-lookup"><span data-stu-id="a7f6b-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="a7f6b-106">Si desidera segnalare falsi positivi o falsi negativi a Microsoft?</span><span class="sxs-lookup"><span data-stu-id="a7f6b-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="a7f6b-107">Utilizzare questo [collegamento](https://www.microsoft.com/wdsi/filesubmission/) per inviare i file per l'analisi.</span><span class="sxs-lookup"><span data-stu-id="a7f6b-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="a7f6b-108">Lo sapevate che è possibile abilitare la protezione dei collegamenti sicuri per la posta elettronica interna inviata tra i destinatari all'interno dell'organizzazione?</span><span class="sxs-lookup"><span data-stu-id="a7f6b-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="a7f6b-109">Eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="a7f6b-109">Follow these steps:</span></span>

  1. <span data-ttu-id="a7f6b-110">Accedere a [https://protection.office.com](https://protection.office.com) e accedere con un account di amministratore globale o amministratore di sicurezza.</span><span class="sxs-lookup"><span data-stu-id="a7f6b-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="a7f6b-111">Nel riquadro di spostamento a sinistra in **gestione minacce**scegliere **Policy** \> **collegamenti sicuri**per i criteri.</span><span class="sxs-lookup"><span data-stu-id="a7f6b-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="a7f6b-112">Nei **criteri che si applicano all'intera sezione organizzazione** selezionare il criterio e fare clic su **modifica**.</span><span class="sxs-lookup"><span data-stu-id="a7f6b-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="a7f6b-113">In **Impostazioni**, abilitare **applica collegamenti sicuri ai messaggi inviati all'interno dell'organizzazione**.</span><span class="sxs-lookup"><span data-stu-id="a7f6b-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
