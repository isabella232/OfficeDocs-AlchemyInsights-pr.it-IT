---
title: Creazione di criteri per le etichette AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542133"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="629db-102">Creazione di criteri per le etichette AIP</span><span class="sxs-lookup"><span data-stu-id="629db-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="629db-103">Le etichette di Azure Information Protection (AIP) possono essere utilizzate con l'intera gamma di dati che un'organizzazione in genere crea e archivia, dalla classificazione più bassa dei dati personali, alla classificazione più elevata di dati altamente riservati.</span><span class="sxs-lookup"><span data-stu-id="629db-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="629db-104">I criteri di protezione delle informazioni di Azure si applicano al client classico di Azure Information Protection (AIP) e non al [client di etichettatura AIP Unified](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="629db-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="629db-105">È possibile configurare più elementi in un criterio di AIP, incluse opzioni quali:</span><span class="sxs-lookup"><span data-stu-id="629db-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="629db-106">Opzione per l'etichetta che consente agli amministratori o agli utenti di classificare e proteggere (facoltativamente) documenti e messaggi di posta elettronica</span><span class="sxs-lookup"><span data-stu-id="629db-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="629db-107">Opzione per applicare la classificazione quando gli utenti salvano documenti e inviano messaggi di posta elettronica</span><span class="sxs-lookup"><span data-stu-id="629db-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="629db-108">Opzione per etichettare automaticamente un messaggio di posta elettronica, in base ai relativi allegati.</span><span class="sxs-lookup"><span data-stu-id="629db-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="629db-109">Opzione per controllare se la barra di protezione delle informazioni viene visualizzata nelle applicazioni di Office</span><span class="sxs-lookup"><span data-stu-id="629db-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="629db-110">Per ulteriori informazioni e opzioni sui criteri di protezione delle informazioni di Azure, vedere: [Overview of the Azure Information Protection Policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="629db-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="629db-111">Per altre risorse utili sui criteri di AIP, vedere:</span><span class="sxs-lookup"><span data-stu-id="629db-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="629db-112">Esercitazione: configurare le impostazioni del criterio di protezione delle informazioni di Azure e creare una nuova etichetta</span><span class="sxs-lookup"><span data-stu-id="629db-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="629db-113">Configurazione dei criteri di protezione delle informazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="629db-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="629db-114">Creare e configurare etichette di riservatezza e i relativi criteri</span><span class="sxs-lookup"><span data-stu-id="629db-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="629db-115">Procedure guidate per scenari comuni in cui viene utilizzata la protezione delle informazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="629db-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="629db-116">Esaminare la documentazione relativa alla protezione delle informazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="629db-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="629db-117">Requisiti per la protezione delle informazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="629db-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="629db-118">Esercitazione introduttiva per la protezione delle informazioni di Azure</span><span class="sxs-lookup"><span data-stu-id="629db-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="629db-119">Scaricare il client Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="629db-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)