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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736686"
---
# <a name="fix-tenant-policy-action-override"></a>Correggere i criteri tenant (override dell'azione)

Questo messaggio è stato influenzato da un criterio di protezione da posta indesiderata nel tenant. Per esaminare il criterio, eseguire le operazioni seguenti:

1. Passare al Centro [sicurezza e & conformità di Office 365 e](https://go.microsoft.com/fwlink/p/?linkid=2077143)quindi a Criteri di gestione delle minacce Protezione da posta   >    >  [indesiderata.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Verificare se **l'origine dei criteri** indica quanto  **segue: Add-Xheader/ModifySubject/Redirect/Delete/No action/BCC message**

    In tal caso, nella **scheda Personalizzata** controllare le impostazioni del criterio che ha interessato il messaggio. È possibile che il messaggio sia stato influenzato dalle impostazioni **Standard** applicate a tutti i clienti di Exchange Online Protection.

Per ulteriori informazioni sulla configurazione dei criteri di filtro della posta indesiderata, vedere [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).
