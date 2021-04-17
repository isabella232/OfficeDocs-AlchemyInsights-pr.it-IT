---
title: 'Scanner AIP: Installazione e configurazione'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821667"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="d4ea8-102">Scanner AIP: Installazione e configurazione</span><span class="sxs-lookup"><span data-stu-id="d4ea8-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="d4ea8-103">**Per installare lo scanner AIP, seguire le linee guida consigliate**:</span><span class="sxs-lookup"><span data-stu-id="d4ea8-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="d4ea8-104">Se si sta eseguendo l'aggiornamento e non viene eseguita un'installazione pulita, accertarsi di aver seguito le linee guida per [aggiornare lo scanner di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) e per i client di etichetta unificata, vedere [Aggiornamento scanner Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="d4ea8-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="d4ea8-105">Verificare che l'utente sia conforme con tutti i [Requisiti per i firewall e le impostazioni dell'infrastruttura di rete](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="d4ea8-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="d4ea8-106">Verificare che i [criteri siano impostati](https://docs.microsoft.com/azure/information-protection/configure-policy) sull'etichettatura automatica o che nel criterio sia presente un'etichetta predefinita.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="d4ea8-107">Assicurarsi che il tipo di file pertinente sia configurato per l'etichetta/protezione come descritto in [Tipi di file supportati dal client di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="d4ea8-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="d4ea8-108">Inoltre, se si vuole modificare il comportamento predefinito, seguire queste linee guida: [Cambiare il livello di protezione predefinito dei file](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="d4ea8-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="d4ea8-109">Verificare che l'account utente configurato per l'esecuzione del servizio scanner disponga delle autorizzazioni necessarie per accedere a tutti i repository configurati.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="d4ea8-110">Se si verificano ancora problemi, esportare i log di scanner e aggiungerli al ticket di supporto.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="d4ea8-111">**Esportare i log dello scanner di Azure Information Protection**</span><span class="sxs-lookup"><span data-stu-id="d4ea8-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="d4ea8-112">Passare a%localappdata%\Microsoft\MSIP nel contesto utente che sta eseguendo il servizio scanner.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="d4ea8-113">Comprimere tutto il contenuto in un file zip nella cartella MSIP.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="d4ea8-114">Salvare i log nella posizione desiderata e allegarli alla richiesta di servizio.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="d4ea8-115">È anche possibile usare [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="d4ea8-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="d4ea8-116">**Per altre informazioni, vedere**:</span><span class="sxs-lookup"><span data-stu-id="d4ea8-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="d4ea8-117">Distribuzione dello strumento di analisi Azure Information Protection per classificare e proteggere automaticamente i file</span><span class="sxs-lookup"><span data-stu-id="d4ea8-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="d4ea8-118">Specificare e usare il parametro token per Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="d4ea8-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="d4ea8-119">Eseguire un ciclo di individuazione e visualizzare i report per lo scanner</span><span class="sxs-lookup"><span data-stu-id="d4ea8-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="d4ea8-120">Consultare la documentazione di Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d4ea8-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="d4ea8-121">Requisiti di Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d4ea8-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="d4ea8-122">Scaricare il client di Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="d4ea8-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
