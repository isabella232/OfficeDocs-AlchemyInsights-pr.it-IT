---
title: Risoluzione dei problemi relativi a Office 365 Advanced Threat Protection (ATP)
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
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511116"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="459b0-102">Risoluzione dei problemi relativi a Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="459b0-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="459b0-103">**Note ritardi con il recapito dei messaggi di posta elettronica**?</span><span class="sxs-lookup"><span data-stu-id="459b0-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="459b0-104">Provare a utilizzare l'opzione per il recapito dinamico per i criteri degli allegati sicuri di ATP.</span><span class="sxs-lookup"><span data-stu-id="459b0-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="459b0-105">In questo modo si eviteranno ritardi nei messaggi di posta elettronica durante la protezione dei destinatari da file dannosi.</span><span class="sxs-lookup"><span data-stu-id="459b0-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="459b0-106">**Si desidera segnalare falsi positivi o falsi negativi**?</span><span class="sxs-lookup"><span data-stu-id="459b0-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="459b0-107">Utilizzare questo collegamento per inviare il file per l'analisi:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="459b0-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="459b0-108">Lo sapevate **che è possibile abilitare la protezione dei collegamenti sicuri ATP per la posta elettronica inviata tra gli utenti dell'organizzazione**?</span><span class="sxs-lookup"><span data-stu-id="459b0-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="459b0-109">Eseguire la procedura seguente:</span><span class="sxs-lookup"><span data-stu-id="459b0-109">Follow these steps:</span></span>
    1. <span data-ttu-id="459b0-110">Vai a https://protection.office.com e accedi.</span><span class="sxs-lookup"><span data-stu-id="459b0-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="459b0-111">Accedere a **Threat management**  >  **Policy**  >  **collegamenti attendibili**dei criteri di gestione delle minacce.</span><span class="sxs-lookup"><span data-stu-id="459b0-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="459b0-112">In **criteri che si applicano a destinatari specifici**, modificare (o aggiungere) un criterio.</span><span class="sxs-lookup"><span data-stu-id="459b0-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="459b0-113">Selezionare **applica collegamenti sicuri ai messaggi inviati all'interno dell'organizzazione**.</span><span class="sxs-lookup"><span data-stu-id="459b0-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="459b0-114">Salvare il criterio e consentire circa 30 minuti affinché le modifiche vengano elaborate tramite il Data Center.</span><span class="sxs-lookup"><span data-stu-id="459b0-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="459b0-115">Per ottenere ulteriori informazioni su ATP, vedere [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span><span class="sxs-lookup"><span data-stu-id="459b0-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>