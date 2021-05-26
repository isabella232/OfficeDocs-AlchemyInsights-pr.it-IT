---
title: Regole per la riduzione della superficie di attacco
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651501"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="d0692-102">Regole per la riduzione della superficie di attacco</span><span class="sxs-lookup"><span data-stu-id="d0692-102">Attack surface reduction rules</span></span>

<span data-ttu-id="d0692-103">L'esclusione di file o cartelle può ridurre in modo grave la protezione fornita dalle regole di riduzione delle superficie di attacco.</span><span class="sxs-lookup"><span data-stu-id="d0692-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="d0692-104">È consentita l'esecuzione dei file che sarebbero stati bloccati da una regola e non vengono registrati report o eventi.</span><span class="sxs-lookup"><span data-stu-id="d0692-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="d0692-105">Un'esclusione si applica a tutte le regole che consentono le esclusioni.</span><span class="sxs-lookup"><span data-stu-id="d0692-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="d0692-106">Le esclusioni di riduzione della superficie di attacco usano la stessa sintassi delle esclusioni di Antivirus Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="d0692-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="d0692-107">Per informazioni dettagliate, vedere [Configurare e convalidare le esclusioni per le analisi di Antivirus Microsoft Defender](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="d0692-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="d0692-108">Per evitare problemi, esaminare [Errori comuni da evitare quando si definiscono le esclusioni](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="d0692-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="d0692-109">Non tutte le regole di riduzione della superficie di attacco supportano le esclusioni.</span><span class="sxs-lookup"><span data-stu-id="d0692-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="d0692-110">Per verificare se la regola supporta le esclusioni, vedere la tabella [Regole per la riduzione della superficie di attacco](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="d0692-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="d0692-111">Regole per la riduzione della superficie di attacco</span><span class="sxs-lookup"><span data-stu-id="d0692-111">Attack surface reduction rules</span></span>

<span data-ttu-id="d0692-112">La superficie di attacco dell'organizzazione include tutte le aree in cui un utente malintenzionato potrebbe compromettere dispositivi o reti aziendali.</span><span class="sxs-lookup"><span data-stu-id="d0692-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="d0692-113">Ridurre la superficie di attacco significa proteggere i dispositivi e la rete dell'organizzazione, lasciando agli utenti malintenzionati meno modi per eseguire gli attacchi.</span><span class="sxs-lookup"><span data-stu-id="d0692-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="d0692-114">Può essere utile configurare regole di riduzione della superficie di attacco in Microsoft Defender per endpoint.</span><span class="sxs-lookup"><span data-stu-id="d0692-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="d0692-115">Per altre informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="d0692-115">For more information, see:</span></span>

- [<span data-ttu-id="d0692-116">Eseguire il mapping del GUID della regola ASR al nome</span><span class="sxs-lookup"><span data-stu-id="d0692-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="d0692-117">Requisiti delle regole ASR:</span><span class="sxs-lookup"><span data-stu-id="d0692-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="d0692-118">Windows 10 Pro, versione 1709 o successiva</span><span class="sxs-lookup"><span data-stu-id="d0692-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="d0692-119">Windows 10 Enterprise, versione 1709 o successiva</span><span class="sxs-lookup"><span data-stu-id="d0692-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="d0692-120">Windows Server, versione 1803 (Canale semestrale) o successiva</span><span class="sxs-lookup"><span data-stu-id="d0692-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="d0692-121">Identificare l'esclusione corretta da applicare</span><span class="sxs-lookup"><span data-stu-id="d0692-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="d0692-122">Cercare eventID 1121 o 1122 nel log Microsoft-Windows-Windows Defender/Operational.</span><span class="sxs-lookup"><span data-stu-id="d0692-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="d0692-123">Valutare lo scenario e il contesto dei blocchi e verificare che lo scenario deve essere sbloccato.</span><span class="sxs-lookup"><span data-stu-id="d0692-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="d0692-124">Leggere il valore Path nei dettagli dell'evento, ovvero il valore che definisce l'esclusione.</span><span class="sxs-lookup"><span data-stu-id="d0692-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="d0692-125">Rendere l'esclusione il più restrittiva possibile.</span><span class="sxs-lookup"><span data-stu-id="d0692-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="d0692-126">Applicare un carattere jolly quando necessario, ad esempio sostituire la variabile User.</span><span class="sxs-lookup"><span data-stu-id="d0692-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="d0692-127">Applicare l'esclusione in base alle esigenze di distribuzione.</span><span class="sxs-lookup"><span data-stu-id="d0692-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="d0692-128">Per informazioni dettagliate, vedere [Personalizzare regole per la riduzione della superficie di attacco](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="d0692-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="d0692-129">L'esclusione non viene rispettata</span><span class="sxs-lookup"><span data-stu-id="d0692-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="d0692-130">Determinare se la regola supporta le esclusioni.</span><span class="sxs-lookup"><span data-stu-id="d0692-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="d0692-131">Per informazioni dettagliate, vedere [Regole per la riduzione della superficie di attacco](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="d0692-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="d0692-132">Esaminare le esclusioni applicate e verificare se i dati dell'evento sono relativi a errori di digitazione o a caratteri jolly non interpretati correttamente.</span><span class="sxs-lookup"><span data-stu-id="d0692-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="d0692-133">Per altre informazioni, vedere i [Tipi di esclusione supportati](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="d0692-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="d0692-134">Se l'impatto della regola è troppo elevato, è consigliabile riportare la regola in modalità di controllo per eseguire ulteriori convalide.</span><span class="sxs-lookup"><span data-stu-id="d0692-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="d0692-135">Per informazioni dettagliate, vedere [Verificare il funzionamento delle funzionalità di Microsoft Defender per endpoint in modalità di controllo](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="d0692-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="d0692-136">Raccogliere dati di supporto per aprire un caso di supporto usando questo comando:</span><span class="sxs-lookup"><span data-stu-id="d0692-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="d0692-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="d0692-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="d0692-138">Per altre informazioni, vedere [Problemi con l’onboarding delle macchine a Microsoft Defender per endpoint](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="d0692-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
