---
title: Creare un messaggio di posta elettronica catch all
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816204"
---
# <a name="create-an-email-catch-all"></a>Creare un messaggio di posta elettronica catch all

L'uso di un catch all è fortemente sconsigliato. È meglio fornire un rimbalzo al mittente, in modo che i mittenti sappiano che il messaggio non può essere recapitato come indirizzato in modo che possano agire. È inoltre possibile limitare la cassetta postale monitorata solo agli indirizzi di posta elettronica validi in precedenza. 

Qualsiasi blocco di tutte le cassette postali riceverà una buona quantità di posta indesiderata e potrebbe eventualmente riempirsi se non strettamente monitorato. Sono previsti limiti di ricezione. 

Se si decide di procedere, attenersi alla seguente procedura:

1. Creare un gruppo di distribuzione dinamico & "Tutti i tipi di destinatari".

2. Creare una cassetta postale dedicata per intercettare i messaggi di posta elettronica, ad esempio, catchall@domain.com.

3. Per il dominio specifico, imposta DomainType su "InternalRelay". Se in seguito si rimuovono tutti i blocchi, assicurarsi di impostare nuovamente il dominio su Autorevole.

4. Creare una regola di trasporto Del flusso di posta come segue:

    - Se il mittente è "Esterno all'organizzazione"
    - Reindirizzare il messaggio a Catchall@domain.com
    - Tranne se il destinatario è un membro di allusers@domain.com (il gruppo di distribuzione contiene tutti i membri)
    - Verificare che le nuove cassette postali siano aggiunte al gruppo di distribuzione dinamico
