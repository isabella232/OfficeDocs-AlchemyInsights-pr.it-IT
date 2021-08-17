---
title: Bloccare le firme di posta elettronica effettuate dall'utente
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: ad743cea4b8735b35b90bd5bf3d0b5b933184ed82858e828a68beb2ca2f8270c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54103556"
---
# <a name="block-user-made-email-signatures"></a>Bloccare le firme di posta elettronica effettuate dall'utente

La soluzione seguente si applica solo alle firme di posta elettronica create in Outlook sul web. Puoi bloccare le firme nell'app Outlook solo se hai un'app locale Exchange Server.

1. Nell'interfaccia di amministrazione scegliere **Interfaccia di amministrazione**  >  **Exchange**.
2. Fare **clic su** autorizzazioni Outlook Web App  >  **criteri.**
3. Selezionare il criterio e quindi fare clic sull'icona a forma di matita per modificarlo.
4. Fare clic **su funzionalità**  >  **Altre opzioni.**
5. In **Esperienza utente** deselezionare la casella di controllo Firma **di** posta elettronica e quindi fare clic su **Salva.**

**Importante:** Se è stata aggiunta una firma prima di deselezionare questa casella di controllo, l'utente potrà comunque utilizzarla. Chiedere loro di rimuoverlo.
