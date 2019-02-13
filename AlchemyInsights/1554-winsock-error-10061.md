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
# <a name="winsock-error-10061"></a>Errori Winsock 10061

Questo codice di errore indica che Office 365 non è stato stabilire un socket TCP (connessione) con l'host di destinazione. La causa più probabile di questo errore è un problema con la configurazione del firewall. Per risolvere il problema, verificare queste impostazioni:
  
- Verificare la configurazione dei firewall con le informazioni contenute in [Office 365 URL e intervalli di indirizzi IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Se l'errore è specifica per Exchange Online Protection (EOP), è consigliabile sono stati precedentemente informati a una modifica gli [indirizzi IP di Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Verificare che il Provider di servizi Internet (ISP) non sia bloccata la porta.
    
- Verificare le impostazioni di server di smart host e di destinazione in dei connettori.
    
Si noti che Office 365 non bloccano le connessioni *in ingresso* in questo modo. 
  

