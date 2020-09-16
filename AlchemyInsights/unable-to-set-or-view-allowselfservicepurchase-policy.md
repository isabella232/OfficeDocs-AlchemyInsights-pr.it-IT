---
title: Impossibile impostare o visualizzare i criteri di AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735203"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="58d43-102">Impossibile impostare o visualizzare i criteri di AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="58d43-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="58d43-103">Quando si tenta di impostare o visualizzare il criterio AllowSelfServicePurchase, viene visualizzato il messaggio di errore seguente:</span><span class="sxs-lookup"><span data-stu-id="58d43-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="58d43-104">*HandleError: failed to retrieve Product Policy with PolicyId ' AllowSelfServicePurchase ', ErrorMessage-la connessione sottostante è stata chiusa: si è verificato un errore imprevisto su un invio.*</span><span class="sxs-lookup"><span data-stu-id="58d43-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="58d43-105">Questo può essere dovuto a una versione precedente di TLS (Transport Layer Security).</span><span class="sxs-lookup"><span data-stu-id="58d43-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="58d43-106">Per connettere il servizio MSCommerce, è necessario utilizzare TLS 1,2 o versione successiva.</span><span class="sxs-lookup"><span data-stu-id="58d43-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="58d43-107">Provare a eseguire la procedura seguente per abilitare o impostare il protocollo TLS su 1,2, verificare e riprovare.</span><span class="sxs-lookup"><span data-stu-id="58d43-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="58d43-108">Al prompt dei comandi di PowerShell (PS C: \) immettere il seguente comando per impostare il protocollo TLS sulla versione 1,2:</span><span class="sxs-lookup"><span data-stu-id="58d43-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="58d43-109">Verificare i protocolli TLS in uso, con il seguente comando:</span><span class="sxs-lookup"><span data-stu-id="58d43-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="58d43-110">Riprovare i comandi Get o Update in base alle esigenze.</span><span class="sxs-lookup"><span data-stu-id="58d43-110">Retry the Get or Update commands as needed.</span></span>

