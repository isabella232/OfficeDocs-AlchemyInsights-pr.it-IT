---
title: Esempio di criterio allegati sicuri di Microsoft Defender per Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736750"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Esempio di criterio allegati sicuri di Microsoft Defender per Office 365

Queste impostazioni abilitano un criterio denominato *Nessun* ritardo che recapita immediatamente i messaggi e quindi ricollegare gli allegati dopo l'analisi:

- **Nome**: Nessun ritardo
- **Descrizione:** recapita immediatamente i messaggi e ricollegare gli allegati dopo l'analisi.
- **Risposta:** selezionare **l'opzione Recapito** dinamico. Per ulteriori informazioni, vedere [Recapito dinamico nei criteri allegati sicuri.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Sezione** Reindirizza allegato: selezionare l'opzione Abilita reindirizzamento **e** quindi immettere l'indirizzo di posta elettronica dell'amministratore globale di Microsoft 365, dell'amministratore della sicurezza o dell'analista della sicurezza che analista della sicurezza analgherà gli allegati dannosi.
- **Sezione Applicato a:** selezionare **Il dominio del destinatario è** e quindi selezionare il dominio. Selezionare **aggiungi** e quindi fare clic su **OK.** Al termine, selezionare **Salva**.

Per ulteriori informazioni, vedere [Allegati sicuri in Microsoft Defender per Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
