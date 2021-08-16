---
title: Esempio di criterio Microsoft Defender per Office 365 Cassaforte allegati
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
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988299"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Esempio di criterio Microsoft Defender per Office 365 Cassaforte allegati

Queste impostazioni abilitano un criterio denominato *Nessun* ritardo che recapita immediatamente i messaggi e quindi ricollegare gli allegati dopo l'analisi:

- **Nome**: Nessun ritardo
- **Descrizione:** recapita immediatamente i messaggi e ricollegare gli allegati dopo l'analisi.
- **Risposta:** selezionare **l'opzione Recapito** dinamico. Per ulteriori informazioni, vedere [Dynamic Delivery in Cassaforte Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).
- **Sezione** Reindirizza allegato: selezionare l'opzione Abilita reindirizzamento **e** quindi immettere l'indirizzo di posta elettronica dell'amministratore globale, dell'amministratore della sicurezza o dell'analista della sicurezza di Microsoft 365 che indagherà su allegati dannosi.
- **Sezione Applicato a:** selezionare **Il dominio del destinatario è** e quindi selezionare il dominio. Selezionare **aggiungi** e quindi fare clic su **OK.** Al termine, selezionare **Salva**.

Per ulteriori informazioni, vedere [Cassaforte allegati in Microsoft Defender per Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).
