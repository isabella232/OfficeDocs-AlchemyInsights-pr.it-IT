---
title: Errore di Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903104"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="46bff-102">Errori Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="46bff-102">Winsock error 10061</span></span>

<span data-ttu-id="46bff-p101">Questo codice di errore indica che Office 365 non è stato stabilire un socket TCP (connessione) con l'host di destinazione. La causa più probabile di questo errore è un problema con la configurazione del firewall. Per risolvere il problema, verificare queste impostazioni:</span><span class="sxs-lookup"><span data-stu-id="46bff-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="46bff-106">Verificare la configurazione dei firewall con le informazioni contenute in [Office 365 URL e intervalli di indirizzi IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="46bff-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="46bff-107">Se l'errore è specifica per Exchange Online Protection (EOP), è consigliabile sono stati precedentemente informati a una modifica gli [indirizzi IP di Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="46bff-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="46bff-108">Verificare che il Provider di servizi Internet (ISP) non sia bloccata la porta.</span><span class="sxs-lookup"><span data-stu-id="46bff-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="46bff-109">Verificare le impostazioni di server di smart host e di destinazione in dei connettori.</span><span class="sxs-lookup"><span data-stu-id="46bff-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="46bff-110">Si noti che Office 365 non bloccano le connessioni *in ingresso* in questo modo.</span><span class="sxs-lookup"><span data-stu-id="46bff-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

