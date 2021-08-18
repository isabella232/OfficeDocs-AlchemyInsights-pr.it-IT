---
title: Correggere i criteri tenant (override dell'azione)
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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326801"
---
# <a name="fix-tenant-policy-action-override"></a>Correggere i criteri tenant (override dell'azione)

Uno dei criteri di protezione da posta indesiderata ha interessato questo messaggio. Per esaminare i criteri, eseguire la procedura seguente:

1. Nel portale Microsoft 365 Defender posta elettronica all'indirizzo , passare a Criteri di collaborazione & e-mail & regole Criteri di minaccia Protezione da posta <https://security.microsoft.com/>  \>  \>  \>  indesiderata nella **sezione** Criteri.

   Per passare direttamente alla pagina **Criteri di protezione dalla posta indesiderata**, usare <https://security.microsoft.com/antispam>.

2. Nella pagina Criteri di protezione da posta indesiderata selezionare il criterio facendo clic sul nome del criterio **(** Type is Custom **anti-spam** **policy** o **Name** is **Anti-Spam inbound policy (Default)**.
3. Nel riquadro a comparsa dei dettagli visualizzato selezionare **Modifica azioni** nella **sezione** Azioni.
4. Nella sezione **Azioni messaggio** esaminare i verdetti relativi a **Spam,** High **confidence spam,** **Phishing** e High **confidence phishing** per verificare se è selezionato uno dei valori seguenti:
   - **Aggiungi X-header**
   - **Anteponi oggetto al testo**
   - **Reindirizza messaggio a indirizzo di posta elettronica**
   - **Elimina messaggio**
   - **Nessuna azione**

   È possibile che le impostazioni **Standard** applicate a tutti i clienti Exchange Online Protection interessati dal messaggio.

Per altre informazioni, vedere [Configurare i criteri di protezione dalla posta indesiderata in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
