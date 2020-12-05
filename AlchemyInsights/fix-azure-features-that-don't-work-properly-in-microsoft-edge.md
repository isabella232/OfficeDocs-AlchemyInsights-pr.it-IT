---
title: Operazioni da eseguire se le funzionalità di Azure non funzionano correttamente in Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576484"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Operazioni da eseguire se le funzionalità di Azure non funzionano correttamente in Microsoft Edge

Microsoft Edge ha [problemi noti](https://go.microsoft.com/fwlink/?linkid=2140608) relativi alle aree di sicurezza e potrebbe influire sul modo in cui gli utenti di Azure accedono all'interfaccia di amministrazione di Windows. Se si verificano problemi con le funzionalità di Azure con Microsoft Edge, provare a eseguire le operazioni seguenti:

1. Fare clic sul pulsante **Start** per cercare le **Opzioni Internet** e selezionarlo.
2. Nella finestra di dialogo **Proprietà Internet** passare alla scheda **sicurezza** .
3. Selezionare l'area **siti attendibili** e quindi fare clic sul pulsante **siti** .
4. Nella finestra di dialogo **siti attendibili** aggiungere l'URL del gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) e quindi fare [https://login.live.com](https://login.live.com) clic su **Chiudi**.
5. Nella finestra di dialogo **Proprietà Internet** passare alla scheda **privacy** .
6. Nella sezione **blocco popup** selezionare **Impostazioni**. Nella finestra di dialogo che si apre, aggiungere l'URL del gateway [https://login.microsoftonline.com](https://login.microsoftonline.com) e [https://login.live.com](https://login.live.com) quindi selezionare **Chiudi**.
