---
title: Protezione da posta indesiderata 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672437"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Risolvere i problemi di recapito per il codice di errore 550 5.4.1 inoltro accesso negato

Questo problema si verifica quando si verifica [se un indirizzo di posta elettronica è valido per impedire effetto palla quando si](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) immette la rete di Office 365. Provare a eseguire le operazioni seguenti:

1. Determinare se il problema è specifico di un intero dominio o di un singolo indirizzo di posta elettronica:
    - Intero dominio: in alcuni casi il dominio deve essere sincronizzato; provare [a impostare il dominio su Internal e quindi di nuovo su autorevole](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Indirizzo di posta elettronica singolo: a volte l'indirizzo deve essere sincronizzato; la modifica dell'indirizzo proxy SMTP e quindi la modifica di nuovo può essere utile.
2. Determinare se il problema è specifico di un gruppo o di una cartella pubblica. Per alcuni tipi di oggetto, è possibile che gli oggetti debbano essere creati manualmente in Azure Active Directory.

Se si ha bisogno di ulteriore assistenza, aprire un ticket di supporto e specificare l'ambito del problema (includidng il tipo di oggetto a cui si sta inviando), in modo da potervi aiutare meglio.