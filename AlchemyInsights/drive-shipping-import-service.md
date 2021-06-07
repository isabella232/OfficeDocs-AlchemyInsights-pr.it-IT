---
title: Spedizione unità nel servizio di importazione di Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721693"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="53172-102">Spedizione unità nel servizio di importazione di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="53172-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="53172-103">Utilizzare Spedizione unità copiando i file PST in un disco rigido e inviando poi tale disco rigido a Microsoft.</span><span class="sxs-lookup"><span data-stu-id="53172-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="53172-104">Per avviare il processo:</span><span class="sxs-lookup"><span data-stu-id="53172-104">To start the job:</span></span>

1. <span data-ttu-id="53172-105">In **Governance delle informazioni** nel Centro conformità Microsoft 365, selezionare **Importa**.</span><span class="sxs-lookup"><span data-stu-id="53172-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="53172-106">Selezionare **Scegli tipo di processo di importazione**, quindi selezionare **Avanti**.</span><span class="sxs-lookup"><span data-stu-id="53172-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="53172-107">Per visualizzare i passaggi dell'opzione di importazione, selezionare **Spedizione dei dischi rigidi a una delle posizioni fisiche**.</span><span class="sxs-lookup"><span data-stu-id="53172-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="53172-108">Ecco alcuni aspetti da ricordare:</span><span class="sxs-lookup"><span data-stu-id="53172-108">Here are some things to remember:</span></span>

- <span data-ttu-id="53172-109">Per importare file PST nelle cassette postali di Microsoft 365, è necessario avere il ruolo di importazione/esportazione di cassette postali in Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="53172-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="53172-110">I file PST maggiori di 20 GB potrebbero influire sulle prestazioni.</span><span class="sxs-lookup"><span data-stu-id="53172-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="53172-111">Sono supportate solo le unità SSD da 2,5 pollici o le unità disco rigido interno SATA II/III da 2,5 o 3,5 pollici.</span><span class="sxs-lookup"><span data-stu-id="53172-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="53172-112">Il disco rigido contenente i file PST deve essere crittografato con BitLocker.</span><span class="sxs-lookup"><span data-stu-id="53172-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="53172-113">Il costo per l'importazione dei file PST nelle cassette postali di Microsoft 365 mediante la spedizione delle unità ammonta a $ 2 (dollari USA) per GB di dati.</span><span class="sxs-lookup"><span data-stu-id="53172-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="53172-114">Per ulteriori informazioni sull'uso del metodo Spedizione unità per l'importazione dei file PST, consultare [Utilizzare Spedizione unità per importare i file PST dell'organizzazione](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span><span class="sxs-lookup"><span data-stu-id="53172-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>