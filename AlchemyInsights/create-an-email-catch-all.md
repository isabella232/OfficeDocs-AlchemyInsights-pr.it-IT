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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080750"
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
