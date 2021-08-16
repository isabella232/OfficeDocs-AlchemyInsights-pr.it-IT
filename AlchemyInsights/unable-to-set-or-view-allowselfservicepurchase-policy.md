---
title: Impossibile impostare o visualizzare il criterio AllowSelfServicePurchase
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
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020196"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>Impossibile impostare o visualizzare il criterio AllowSelfServicePurchase

Quando si tenta di impostare o visualizzare il criterio AllowSelfServicePurchase, viene visualizzato il seguente messaggio di errore:

*HandleError: impossibile recuperare i criteri di prodotto con PolicyId 'AllowSelfServicePurchase', ErrorMessage - La connessione sottostante è stata chiusa: si è verificato un errore imprevisto durante un invio.*

Ciò potrebbe essere dovuto a una versione precedente di Transport Layer Security (TLS). Per connettere il servizio MS Commerce, è necessario utilizzare TLS 1.2 o versione successiva.  

Provare la procedura seguente per abilitare/impostare il protocollo TLS su 1.2, verificare e riprovare.
 1. Al prompt dei comandi di PowerShell (PS C: immettere il comando seguente per impostare il \) protocollo TLS sulla versione 1.2:

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. Verificare i protocolli TLS in uso, con il comando seguente:

    `[Net.ServicePointManager]::SecurityProtocol` 

3. Ritentare i comandi Get o Update in base alle esigenze.

