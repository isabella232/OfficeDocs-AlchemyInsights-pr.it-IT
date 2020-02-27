---
title: Creare un messaggio di posta elettronica catch all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286197"
---
# <a name="create-an-email-catch-all"></a>Creare un messaggio di posta elettronica catch all

L'utilizzo di un catch all è fortemente scoraggiato. È preferibile fornire un rimbalzo al mittente affinché i mittenti siano a conoscenza del messaggio che non è stato possibile recapitare come indirizzato in modo che possano intervenire. È inoltre possibile limitare la cassetta postale monitorata solo per rilevare gli indirizzi di posta elettronica precedentemente validi. 

Qualsiasi catch tutte le cassette postali riceverà una buona dose di posta indesiderata e potrebbe eventualmente essere compilato se non monitorato. (Ci sono limiti di ricezione). 

Se si decide di procedere, attenersi alla seguente procedura:

1. Creare un gruppo di distribuzione dinamico & includere "tutti i tipi di destinatari".

2. Creare una cassetta postale dedicata per la cattura di messaggi di posta elettronica, ad esempio, catchall@domain.com.

3. Per il dominio specifico, impostare DomainType su "InternalRelay". Se in seguito si rimuove il blocco tutto, assicurarsi di impostare di nuovo il dominio su autorevole.

4. Creare una regola di trasporto del flusso di posta come indicato di seguito:

    - Se il mittente è "all'esterno dell'organizzazione"
    - Reindirizzare il messaggio a Catchall@domain.com
    - Eccetto se il destinatario è un membro di allusers@domain.com (il gruppo di distribuzione contiene tutti i membri)
    - Assicurarsi di verificare che nuove cassette postali vengano aggiunte al gruppo di distribuzione dinamico
