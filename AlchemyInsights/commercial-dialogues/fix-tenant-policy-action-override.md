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
ms.openlocfilehash: 9c0b88c1ca2120acccd9cd75eb918a81bde52ec3919f6148922f077f07899da7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034938"
---
# <a name="fix-tenant-policy-action-override"></a>Correggere i criteri tenant (override dell'azione)

Questo messaggio è stato influenzato da un criterio di protezione da posta indesiderata nel tenant. Per esaminare il criterio, eseguire le operazioni seguenti:

1. Passare al Centro [Office 365 sicurezza &](https://go.microsoft.com/fwlink/p/?linkid=2077143)e quindi passare a Criteri di gestione delle minacce Protezione da posta  >    >  [indesiderata.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Verificare se **l'origine dei criteri** indica quanto  **segue: Add-Xheader/ModifySubject/Redirect/Delete/No action/BCC message**

    In tal caso, nella **scheda Personalizzata** controllare le impostazioni del criterio che ha interessato il messaggio. È possibile che le impostazioni **Standard applicate** a tutti i clienti Exchange Online Protection interessati dal messaggio.

Per ulteriori informazioni sulla configurazione dei criteri di filtro della posta indesiderata, vedere [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).
