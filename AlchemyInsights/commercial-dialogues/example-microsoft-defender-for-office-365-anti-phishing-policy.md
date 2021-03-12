---
title: Esempio di criterio anti-phishing di Microsoft Defender per Office 365
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/11/2021
ms.locfileid: "50737185"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Esempio di criterio anti-phishing di Microsoft Defender per Office 365

Queste impostazioni abilitano un criterio *denominato Dominio e CEO.* Questo criterio fornisce protezione utente e dominio dalla rappresentazione e quindi applica il criterio a tutti i messaggi di posta elettronica ricevuti dagli utenti all'interno del dominio. Innanzitutto, aggiungere le informazioni seguenti per creare il criterio:

- **Name**: Domain and CEO **Description**: Garantisce che il CEO e il dominio non vengano impersonati.
  **Applicato a**: selezionare **Il dominio del destinatario è**. In **Uno di questi,** selezionare **Scegli** e quindi selezionare un dominio. Selezionare **+ Aggiungi**. Selezionare la casella di controllo accanto al nome del dominio nell'elenco , ad esempio *contoso.com*), quindi selezionare **Aggiungi**. Scegliere **Fatto**.
- Dopo aver creato il criterio, è possibile ottimizzare il criterio utilizzando le opzioni seguenti:
  - **Aggiungere utenti da proteggere:** Per questo esempio, aggiungi almeno l'indirizzo di posta elettronica del CEO.
  - **Aggiungere domini da proteggere:** aggiungere il dominio dell'organizzazione che include l'ufficio del CEO.
  - **Scegliere azioni**: **Per** Se la posta elettronica viene inviata da un utente *rappresentato,* selezionare Reindirizza il messaggio a un altro indirizzo **di** posta elettronica e quindi immettere l'indirizzo di posta elettronica dell'amministratore della sicurezza (ad esempio, securityadmin@contoso.com ). Per **Se la posta elettronica viene inviata da un dominio rappresentato,** selezionare **Metti in quarantena il messaggio.**
  - **Intelligence delle** cassette postali: per impostazione predefinita, questa opzione è selezionata quando si crea un nuovo criterio anti-phishing. Per ottenere risultati ottimali, lasciare l’opzione **attiva**.
  - **Aggiungere mittenti e domini attendibili:** Per questo esempio, non definire sostituzioni.
- Dopo aver esaminato le impostazioni, selezionare **Crea questo criterio** o **Salva**, come appropriato.

Per ulteriori informazioni, vedere [Criteri anti-phishing in Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
