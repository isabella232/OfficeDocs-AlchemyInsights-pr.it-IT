---
title: Creazione di criteri per le etichette AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732179"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="a6498-102">Creazione di criteri per le etichette AIP</span><span class="sxs-lookup"><span data-stu-id="a6498-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="a6498-103">Le etichette di Azure Information Protection (AIP) possono essere utilizzate con l'intera gamma di dati che un'organizzazione in genere crea e archivia, dalla classificazione più bassa dei dati personali, alla classificazione più elevata di dati altamente riservati.</span><span class="sxs-lookup"><span data-stu-id="a6498-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="a6498-104">I criteri di protezione delle informazioni di Azure si applicano al client classico di Azure Information Protection (AIP) e non al  [client di etichettatura AIP Unified](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="a6498-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="a6498-105">È possibile configurare più elementi in un criterio di AIP, incluse opzioni quali:</span><span class="sxs-lookup"><span data-stu-id="a6498-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="a6498-106">Opzione per l'etichetta che consente agli amministratori o agli utenti di classificare e proteggere (facoltativamente) documenti e messaggi di posta elettronica</span><span class="sxs-lookup"><span data-stu-id="a6498-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="a6498-107">Opzione per applicare la classificazione quando gli utenti salvano documenti e inviano messaggi di posta elettronica</span><span class="sxs-lookup"><span data-stu-id="a6498-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="a6498-108">Opzione per etichettare automaticamente un messaggio di posta elettronica, in base ai relativi allegati.</span><span class="sxs-lookup"><span data-stu-id="a6498-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="a6498-109">Opzione per controllare se la barra di protezione delle informazioni viene visualizzata nelle applicazioni di Office</span><span class="sxs-lookup"><span data-stu-id="a6498-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="a6498-110">Per ulteriori informazioni e opzioni sui criteri di protezione delle informazioni di Azure, vedere: [Overview of the Azure Information Protection Policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="a6498-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="a6498-111">Per altre risorse utili sui criteri di AIP, vedere:</span><span class="sxs-lookup"><span data-stu-id="a6498-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="a6498-112">Tutorial: configurare le impostazioni dei criteri di Azure Information Protection e creare una nuova etichetta</span><span class="sxs-lookup"><span data-stu-id="a6498-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a6498-113">Configurazione dei criteri di Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a6498-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="a6498-114">Creare e configurare etichette di riservatezza e i relativi criteri</span><span class="sxs-lookup"><span data-stu-id="a6498-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="a6498-115">Guide sulle procedure per scenari comuni che usano Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a6498-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="a6498-116">Consultare la documentazione di Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a6498-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="a6498-117">Requisiti di Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a6498-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="a6498-118">Guida introduttiva per Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a6498-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a6498-119">Scaricare il client di Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="a6498-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)