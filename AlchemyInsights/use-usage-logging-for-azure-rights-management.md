---
title: Usare la registrazione dell'utilizzo per Azure Rights Management
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/03/2020
ms.locfileid: "46543774"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="07465-102">Usare la registrazione dell'utilizzo per Azure Rights Management</span><span class="sxs-lookup"><span data-stu-id="07465-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="07465-103">Per impostazione predefinita, la registrazione dell'utilizzo delle protezioni è abilitata per tutti i clienti.</span><span class="sxs-lookup"><span data-stu-id="07465-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="07465-104">I log sono scritti come una serie di BLOB nello spazio di archiviazione di Azure per il proprio tenant.</span><span class="sxs-lookup"><span data-stu-id="07465-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="07465-105">Dopo un'azione di protezione, bisogna attendere fino a 15 minuti prima che la maggior parte dei log sia visualizzata.</span><span class="sxs-lookup"><span data-stu-id="07465-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="07465-106">È possibile usare i log dell'utilizzo delle protezioni per:</span><span class="sxs-lookup"><span data-stu-id="07465-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="07465-107">Analizzare dati commerciali</span><span class="sxs-lookup"><span data-stu-id="07465-107">Analyze business insights</span></span>

- <span data-ttu-id="07465-108">Controllare gli abusi</span><span class="sxs-lookup"><span data-stu-id="07465-108">Monitor for abuse</span></span>

- <span data-ttu-id="07465-109">Eseguire analisi forensi</span><span class="sxs-lookup"><span data-stu-id="07465-109">Perform forensic analysis</span></span>

<span data-ttu-id="07465-110">Per altre informazioni, vedere [Registrare e analizzare l'utilizzo delle protezioni di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span><span class="sxs-lookup"><span data-stu-id="07465-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="07465-111">Per informazioni sulla registrazione dell'utilizzo dei client, vedere [Guida per amministratori: registrazione dell'utilizzo e dei file dei client di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span><span class="sxs-lookup"><span data-stu-id="07465-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="07465-112">Per altre informazioni, vedere:</span><span class="sxs-lookup"><span data-stu-id="07465-112">For additional information, see:</span></span>

- <span data-ttu-id="07465-113">[Requisiti di Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)</span><span class="sxs-lookup"><span data-stu-id="07465-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="07465-114">[Tutorial: configurare le impostazioni dei criteri di Azure Information Protection e creare una nuova etichetta](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span><span class="sxs-lookup"><span data-stu-id="07465-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>