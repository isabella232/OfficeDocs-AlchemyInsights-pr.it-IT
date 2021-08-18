---
title: Correggere i criteri di filtro lingua/IP
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
ms.openlocfilehash: 25744bee6f3ed06ae67fc3c246c7d64fce9994bb
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320529"
---
# <a name="fix-languageip-filter-policy"></a>Correggere i criteri di filtro lingua/IP

Uno dei criteri di protezione da posta indesiderata ha interessato questo messaggio. Per esaminare i criteri, eseguire la procedura seguente:

1. Nel portale Microsoft 365 Defender posta elettronica all'indirizzo , passare a Criteri di collaborazione & e-mail & regole Criteri di minaccia Protezione da posta <https://security.microsoft.com/>  \>  \>  \>  indesiderata nella **sezione** Criteri.

   Per passare direttamente alla pagina **Criteri di protezione dalla posta indesiderata**, usare <https://security.microsoft.com/antispam>.

2. Nella pagina Criteri di protezione da posta indesiderata selezionare il criterio facendo clic sul nome del criterio **(** Type is Custom **anti-spam** **policy** o **Name** is **Anti-Spam inbound policy (Default)**.
3. Nel riquadro a comparsa dei dettagli visualizzato selezionare Modifica **la** soglia e le proprietà della posta indesiderata nella sezione Soglia di posta elettronica in blocco & proprietà della **posta indesiderata.**
4. Nella sezione **Contrassegna come posta** indesiderata esaminare le **impostazioni Contiene lingue specifiche** e Da **questi** paesi.

Per altre informazioni, vedere [Configurare i criteri di protezione dalla posta indesiderata in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
