---
title: Configurazione delle esclusioni per l’analisi di Microsoft Defender ATP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543689"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="99e4f-102">Configurazione delle esclusioni per l’analisi di Microsoft Defender ATP</span><span class="sxs-lookup"><span data-stu-id="99e4f-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="99e4f-103">In generale, è possibile escludere determinate estensioni di file e posizioni delle cartelle dalle analisi di Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="99e4f-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="99e4f-104">È anche possibile configurare le esclusioni per i file che vengono aperti da determinati processi.</span><span class="sxs-lookup"><span data-stu-id="99e4f-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="99e4f-105">Per altre informazioni, vedere [Configurare e convalidare le esclusioni in base all’estensione dei file e alle posizioni delle cartelle](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) e [Configurare le esclusioni per i file aperti da processi](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="99e4f-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="99e4f-106">Per configurare le esclusioni per  **Windows Server 2016 e 2019**, vedere [Configurare le esclusioni di Microsoft Defender Antivirus in Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="99e4f-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="99e4f-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="99e4f-107">**Mac**</span></span>

<span data-ttu-id="99e4f-108">Per informazioni sui tipi di esclusione supportati e sulla configurazione di un elenco di esclusioni per Mac, vedere [Tipi di esclusione supportati](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) e [Come configurare l'elenco delle esclusioni](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="99e4f-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="99e4f-109">**Nota:** è anche possibile convalidare gli elenchi di esclusioni tramite il file di test di EICAR.</span><span class="sxs-lookup"><span data-stu-id="99e4f-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="99e4f-110">Per altre informazioni, vedere [Convalidare gli elenchi di esclusioni con il file di test di EICAR](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="99e4f-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="99e4f-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="99e4f-111">**Linux**</span></span>

<span data-ttu-id="99e4f-112">Per informazioni sui tipi di esclusione supportati e sulla configurazione di un elenco di esclusioni per Linux, vedere [Tipi di esclusione supportati](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) e [Configurare e convalidare le esclusioni per Microsoft Defender ATP per Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="99e4f-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="99e4f-113">**Nota:** è anche possibile convalidare gli elenchi di esclusioni tramite il file di test di EICAR.</span><span class="sxs-lookup"><span data-stu-id="99e4f-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="99e4f-114">Per altre informazioni, vedere [Convalidare gli elenchi di esclusioni con il file di test di EICAR](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="99e4f-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 