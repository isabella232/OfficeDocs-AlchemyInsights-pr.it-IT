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
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232751"
---
# <a name="block-user-made-email-signatures"></a>Bloccare le firme di posta elettronica effettuate dall'utente

La soluzione seguente si applica solo alle firme di posta elettronica create in Outlook sul Web. È possibile bloccare le firme nell'app Outlook solo se si dispone di un Exchange Server.

1. Nell'interfaccia di amministrazione scegliere **Interfaccia di amministrazione di**  >  **Exchange.**
2. Fare clic **su Autorizzazioni** criteri di Outlook  >  **Web App.**
3. Selezionare il criterio e quindi fare clic sull'icona della matita per modificarlo.
4. Fare clic **su funzionalità**  >  **Altre opzioni.**
5. In **Esperienza utente** deselezionare la casella di controllo Firma **di** posta elettronica e quindi fare clic su **Salva.**

**Importante:** Se una firma è stata aggiunta prima di deselezionare questa casella di controllo, l'utente potrà comunque utilizzarla. Chiedere loro di rimuoverlo.
