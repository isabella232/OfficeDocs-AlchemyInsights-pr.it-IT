---
title: Correggere i criteri di connessione
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737140"
---
# <a name="fix-connection-policy"></a>Correggere i criteri di connessione

Il messaggio di posta elettronica è stato contrassegnato come sicuro e recapitato nella posta in arrivo dell'utente perché l'indirizzo IP di invio è stato contrassegnato come sicuro nel criterio Filtro connessioni. Per esaminare il criterio, eseguire le operazioni seguenti:

1. Passare al Centro [sicurezza e & conformità di Office 365 e](https://go.microsoft.com/fwlink/p/?linkid=2077143)quindi a Criteri di gestione delle minacce Protezione da posta   >    >  [indesiderata.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Nella scheda **Personalizzata** selezionare il criterio Filtro **connessioni** e quindi **selezionare Modifica criterio.**
3. Esaminare **l'elenco indirizzi IP** consentiti. Verificare se **l'elenco indirizzi attendibili** è abilitato.

    > [!NOTE]
    > Microsoft sottoscrive origini di terze parti di mittenti attendibili. Se **l'elenco** indirizzi attendibili è abilitato, questi mittenti attendibili non vengono erroneamente contrassegnati come posta indesiderata. È consigliabile selezionare questa opzione perché ridurrà il numero di falsi positivi (buona posta classificata come posta indesiderata) ricevuti.
