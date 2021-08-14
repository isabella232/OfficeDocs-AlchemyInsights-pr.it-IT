---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932281"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Risolvere i problemi di recapito per il codice di errore 550 5.4.1 Relay Access Denied

Questo problema si verifica quando si controlla se un indirizzo di posta elettronica è valido per evitare [rimbalzi](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) quando si entra nella rete Microsoft. Provare a eseguire le operazioni seguenti:

1. Determinare se il problema è specifico di un intero dominio o di un singolo indirizzo di posta elettronica:
    - Intero dominio: a volte il dominio deve essere sincronizzato; provare [a impostare il dominio su Internal e quindi di nuovo su Authoritative.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Indirizzo di posta elettronica singolo: a volte l'indirizzo deve essere sincronizzato; la modifica dell'indirizzo proxy smtp e quindi la modifica di nuovo può essere utile.
2. Determinare se il problema è specifico di un gruppo o di una cartella pubblica. Per alcuni tipi di oggetto, potrebbe essere necessario creare manualmente gli oggetti in Azure Active Directory.

Se hai bisogno di ulteriore assistenza, apri un ticket di supporto e specifica l'ambito del problema (incluso il tipo di oggetto a cui stai inviando) in modo che possiamo aiutarti meglio.