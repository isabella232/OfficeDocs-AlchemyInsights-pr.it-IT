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
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091722"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Impossibile impostare o visualizzare i criteri di AllowSelfServicePurchase

Quando si tenta di impostare o visualizzare il criterio AllowSelfServicePurchase, viene visualizzato il messaggio di errore seguente:

*HandleError: failed to retrieve Product Policy with PolicyId ' AllowSelfServicePurchase ', ErrorMessage-la connessione sottostante è stata chiusa: si è verificato un errore imprevisto su un invio.*

Questo può essere dovuto a una versione precedente di TLS (Transport Layer Security). Per connettere il servizio MSCommerce, è necessario utilizzare TLS 1,2 o versione successiva.  

Provare a eseguire la procedura seguente per abilitare o impostare il protocollo TLS su 1,2, verificare e riprovare.
 1. Al prompt dei comandi di PowerShell (PS C\) : immettere il seguente comando per impostare il protocollo TLS sulla versione 1,2:

    \[NET. ServicePointManager]:: SecurityProtocol = \[NET. SecurityProtocolType]:: Tls12

2. Verificare i protocolli TLS in uso, con il seguente comando:

    \[NET. ServicePointManager]:: SecurityProtocol 

3. Riprovare i comandi Get o Update in base alle esigenze.

