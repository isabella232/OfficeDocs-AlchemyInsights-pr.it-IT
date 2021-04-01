---
title: EndPoint Manager - Baseline di sicurezza
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440888"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="a4968-102">EndPoint Manager - Baseline di sicurezza</span><span class="sxs-lookup"><span data-stu-id="a4968-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="a4968-103">Le baseline di sicurezza sono gruppi preconfigurati di impostazioni di Windows che consentono di applicare le impostazioni di sicurezza consigliate dai team di sicurezza pertinenti.</span><span class="sxs-lookup"><span data-stu-id="a4968-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="a4968-104">Queste baseline possono essere personalizzate in modo da fornire solo le impostazioni e i valori desiderati.</span><span class="sxs-lookup"><span data-stu-id="a4968-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="a4968-105">Per altre informazioni sulle baseline di sicurezza, vedere [Usare le baseline di sicurezza per configurare i dispositivi Windows 10 in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="a4968-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="a4968-106">Attualmente sono disponibili baseline per questi prodotti:</span><span class="sxs-lookup"><span data-stu-id="a4968-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="a4968-107">Impostazioni di sicurezza di Windows MDM</span><span class="sxs-lookup"><span data-stu-id="a4968-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="a4968-108">Sicurezza di Microsoft Defender per endpoint</span><span class="sxs-lookup"><span data-stu-id="a4968-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="a4968-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="a4968-109">Microsoft Edge</span></span>

<span data-ttu-id="a4968-110">Ognuna delle baseline viene aggiornata periodicamente e rilasciata in versioni incrementali.</span><span class="sxs-lookup"><span data-stu-id="a4968-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="a4968-111">Ogni versione aggiunge e/o rimuove le impostazioni della versione precedente per garantire che la baseline soddisfi le indicazioni correnti.</span><span class="sxs-lookup"><span data-stu-id="a4968-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="a4968-112">La console Baseline di sicurezza in Sicurezza degli endpoint consente di confrontare versioni diverse rendendo visibili le modifiche da una versione all'altra.</span><span class="sxs-lookup"><span data-stu-id="a4968-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="a4968-113">Per indicazioni su come modificare in modo più efficace la versione della baseline distribuita, vedere [Gestire i profili della baseline di sicurezza in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="a4968-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="a4968-114">Dopo aver distribuito una baseline di sicurezza, è possibile monitorare lo stato della distribuzione ed esaminare le impostazioni a seconda dei dispositivi.</span><span class="sxs-lookup"><span data-stu-id="a4968-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="a4968-115">**Nota:** la visualizzazione dei dati dei report per le baseline può richiedere fino a 24 ore dalla distribuzione iniziale in un dispositivo e fino a 6 ore per ulteriori aggiornamenti.</span><span class="sxs-lookup"><span data-stu-id="a4968-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="a4968-116">La causa più comune per cui un'impostazione della baseline non viene applicata è perché la stessa impostazione viene usata in un profilo diverso.</span><span class="sxs-lookup"><span data-stu-id="a4968-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="a4968-117">Questo scenario può essere esaminato per un dispositivo specifico selezionando tale dispositivo nel nodo Stato dispositivo del profilo Baseline di sicurezza.</span><span class="sxs-lookup"><span data-stu-id="a4968-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="a4968-118">Per informazioni dettagliate, vedere [Risolvere i conflitti per le baseline di sicurezza](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="a4968-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>