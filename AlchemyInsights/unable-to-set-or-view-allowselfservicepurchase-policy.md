---
title: Impossibile impostare o visualizzare i criteri di AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158565"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="139dd-102">Impossibile impostare o visualizzare i criteri di AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="139dd-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="139dd-103">Quando si tenta di impostare o visualizzare il criterio AllowSelfServicePurchase, viene visualizzato il messaggio di errore seguente:</span><span class="sxs-lookup"><span data-stu-id="139dd-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="139dd-104">*HandleError: failed to retrieve Product Policy with PolicyId ' AllowSelfServicePurchase ', ErrorMessage-la connessione sottostante è stata chiusa: si è verificato un errore imprevisto su un invio.*</span><span class="sxs-lookup"><span data-stu-id="139dd-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="139dd-105">Questo può essere dovuto a una versione precedente di TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="139dd-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="139dd-106">Per connettere il servizio MSCommerce, è necessario utilizzare TLS 1,2 o versione successiva.</span><span class="sxs-lookup"><span data-stu-id="139dd-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="139dd-107">Provare a eseguire la procedura seguente per abilitare o impostare il protocollo TLS su 1,2, verificare e riprovare.</span><span class="sxs-lookup"><span data-stu-id="139dd-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="139dd-108">Al prompt dei comandi di PowerShell (PS C\) : immettere il seguente comando per impostare il protocollo TLS sulla versione 1,2:</span><span class="sxs-lookup"><span data-stu-id="139dd-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="139dd-109">Verificare i protocolli TLS in uso, con il seguente comando:</span><span class="sxs-lookup"><span data-stu-id="139dd-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="139dd-110">Riprovare i comandi Get o Update in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="139dd-110">Retry the Get or Update commands as needed.</span></span>

