---
title: Impossibile impostare o visualizzare il criterio AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826095"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="28ed3-102">Impossibile impostare o visualizzare il criterio AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="28ed3-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="28ed3-103">Quando si tenta di impostare o visualizzare il criterio AllowSelfServicePurchase, viene visualizzato il seguente messaggio di errore:</span><span class="sxs-lookup"><span data-stu-id="28ed3-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="28ed3-104">*HandleError: impossibile recuperare i criteri di prodotto con PolicyId 'AllowSelfServicePurchase', ErrorMessage - La connessione sottostante è stata chiusa: si è verificato un errore imprevisto durante un invio.*</span><span class="sxs-lookup"><span data-stu-id="28ed3-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="28ed3-105">Ciò potrebbe essere dovuto a una versione precedente di Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="28ed3-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="28ed3-106">Per connettere il servizio MS Commerce, è necessario utilizzare TLS 1.2 o versione successiva.</span><span class="sxs-lookup"><span data-stu-id="28ed3-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="28ed3-107">Provare la procedura seguente per abilitare/impostare il protocollo TLS su 1.2, verificare e riprovare.</span><span class="sxs-lookup"><span data-stu-id="28ed3-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="28ed3-108">Al prompt dei comandi di PowerShell (PS C: immettere il comando seguente per impostare il \) protocollo TLS sulla versione 1.2:</span><span class="sxs-lookup"><span data-stu-id="28ed3-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="28ed3-109">Verificare i protocolli TLS in uso, con il comando seguente:</span><span class="sxs-lookup"><span data-stu-id="28ed3-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="28ed3-110">Ritentare i comandi Get o Update in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="28ed3-110">Retry the Get or Update commands as needed.</span></span>

