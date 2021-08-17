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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888410"
---
# <a name="fix-connection-policy"></a>Correggere i criteri di connessione

Il messaggio di posta elettronica è stato contrassegnato come sicuro e recapitato nella cartella Posta in arrivo dell'utente perché l'indirizzo IP di origine è stato contrassegnato come sicuro nel criterio filtro connessioni predefinito. Per esaminare il criterio, eseguire la procedura seguente:

1. Nel portale Microsoft 365 Defender posta elettronica all'indirizzo , passare a Email <https://security.microsoft.com/> **& Collaboration** Policies & \> **Rules Threat** \> **policies** \> **Anti-spam** nella **sezione Criteri.**

   Per passare direttamente alla pagina **Criteri di protezione dalla posta indesiderata**, usare <https://security.microsoft.com/antispam>.

2. Nella pagina **Criteri di protezione** da posta indesiderata selezionare il criterio denominato Criterio filtro connessioni **(impostazione predefinita)** facendo clic sul nome del criterio.

3. Nel riquadro a comparsa dei dettagli visualizzato fare clic **su Modifica** criterio filtro connessioni nella **sezione Filtro** connessioni.

4. Esaminare le voci nella sezione **Consenti** sempre messaggi dai seguenti indirizzi IP o intervalli di indirizzi e verificare se l'opzione Attiva elenco **indirizzi** attendibili è selezionata.

   > [!NOTE]
   > Microsoft sottoscrive origini di terze parti di mittenti attendibili. Se l'elenco indirizzi attendibili è abilitato, questi mittenti attendibili non vengono erroneamente contrassegnati come posta indesiderata. È consigliabile selezionare questa opzione perché ridurrà il numero di falsi positivi (buona posta classificata come posta indesiderata) ricevuti.

Per ulteriori informazioni, vedere [Configurare il filtraggio delle connessioni](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
