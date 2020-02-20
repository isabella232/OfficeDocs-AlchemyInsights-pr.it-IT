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
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Impossibile impostare o visualizzare i criteri di AllowSelfServicePurchase

Quando si tenta di impostare o visualizzare il criterio AllowSelfServicePurchase, viene visualizzato il messaggio di errore seguente:

*HandleError: failed to retrieve Product Policy with PolicyId ' AllowSelfServicePurchase ', ErrorMessage-la connessione sottostante è stata chiusa: si è verificato un errore imprevisto su un invio.*

Questo può essere dovuto a una versione precedente di TLS (Transport Layer Security). Per connettere il servizio MSCommerce, è necessario utilizzare TLS 1,2 o versione successiva.  

Provare a eseguire la procedura seguente per abilitare o impostare il protocollo TLS su 1,2, verificare e riprovare.
 1. Al prompt dei comandi di PowerShell (PS C\) : immettere il seguente comando per impostare il protocollo TLS sulla versione 1,2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verificare i protocolli TLS in uso, con il seguente comando:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Riprovare i comandi Get o Update in base alle esigenze.

