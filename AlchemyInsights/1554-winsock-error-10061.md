---
title: Errore di Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/24/2019
ms.locfileid: "29475983"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="dc932-102">Errori Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="dc932-102">Winsock error 10061</span></span>

<span data-ttu-id="dc932-p101">Questo codice di errore indica che Office 365 non è stato stabilire un socket TCP (connessione) con l'host di destinazione. La causa più probabile di questo errore è un problema con la configurazione del firewall. Per risolvere il problema, verificare queste impostazioni:</span><span class="sxs-lookup"><span data-stu-id="dc932-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="dc932-106">Verificare la configurazione dei firewall con le informazioni contenute in [Office 365 URL e intervalli di indirizzi IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="dc932-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="dc932-107">Se l'errore è specifica per Exchange Online Protection (EOP), è consigliabile sono stati precedentemente informati a una modifica gli [indirizzi IP di Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="dc932-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="dc932-108">Verificare che il Provider di servizi Internet (ISP) non sia bloccata la porta.</span><span class="sxs-lookup"><span data-stu-id="dc932-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="dc932-109">Verificare le impostazioni di server di smart host e di destinazione in dei connettori.</span><span class="sxs-lookup"><span data-stu-id="dc932-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="dc932-110">Si noti che Office 365 non bloccano le connessioni *in ingresso* in questo modo.</span><span class="sxs-lookup"><span data-stu-id="dc932-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

