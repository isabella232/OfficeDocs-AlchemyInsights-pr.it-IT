---
title: Esempio di criterio Allegati sicuri di Microsoft Defender per Office 365
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
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530227"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Esempio di criterio Allegati sicuri di Microsoft Defender per Office 365

Queste impostazioni abilitano un criterio denominato *Nessun* ritardo che recapita immediatamente i messaggi e quindi ricollegare gli allegati dopo l'analisi:

- **Name**: No delays
- **Descrizione:** recapita immediatamente i messaggi e ricollegare gli allegati dopo l'analisi.
- **Risposta:** selezionare **l'opzione Recapito** dinamico. Per ulteriori informazioni, vedere [Recapito dinamico nei criteri allegati sicuri.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Sezione** Reindirizza allegato: selezionare l'opzione Abilita reindirizzamento, quindi immettere l'indirizzo di posta elettronica dell'amministratore globale, dell'amministratore della sicurezza o dell'analista della sicurezza di Microsoft 365 che analgherà gli allegati dannosi.
- **Sezione Applicato a:** Selezionare **il dominio del destinatario è** e quindi selezionare il dominio. Selezionare **aggiungi** e quindi fare clic su **OK.** Al termine, selezionare **Salva.**

Per altre informazioni, vedere [Allegati sicuri in Microsoft Defender per Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)
