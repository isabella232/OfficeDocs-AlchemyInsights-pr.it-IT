---
title: Esempio di Microsoft Defender per Office 365 anti-phishing
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035010"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Esempio di Microsoft Defender per Office 365 anti-phishing

Queste impostazioni abilitano un criterio *denominato Dominio e CEO.* Questo criterio fornisce protezione utente e dominio dalla rappresentazione e quindi applica il criterio a tutti i messaggi di posta elettronica ricevuti dagli utenti all'interno del dominio. Innanzitutto, aggiungere le informazioni seguenti per creare il criterio:

- **Name**: Domain and CEO **Description**: Garantisce che il CEO e il dominio non vengano impersonati.
  **Applicato a**: selezionare **Il dominio del destinatario è**. In **Uno di questi,** selezionare **Scegli** e quindi selezionare un dominio. Selezionare **+ Aggiungi**. Selezionare la casella di controllo accanto al nome del dominio nell'elenco , ad esempio *contoso.com*), quindi selezionare **Aggiungi**. Scegliere **Fine**.
- Dopo aver creato il criterio, è possibile ottimizzare il criterio utilizzando le opzioni seguenti:
  - **Aggiungere utenti da proteggere:** Per questo esempio, aggiungi almeno l'indirizzo di posta elettronica del CEO.
  - **Aggiungere domini da proteggere:** aggiungere il dominio dell'organizzazione che include l'ufficio del CEO.
  - **Scegliere azioni**: **Per** Se la posta elettronica viene inviata da un utente *rappresentato,* selezionare Reindirizza il messaggio a un altro indirizzo **di** posta elettronica e quindi immettere l'indirizzo di posta elettronica dell'amministratore della sicurezza (ad esempio, securityadmin@contoso.com ). Per **Se la posta elettronica viene inviata da un dominio rappresentato,** selezionare **Metti in quarantena il messaggio.**
  - **Intelligence delle** cassette postali: per impostazione predefinita, questa opzione è selezionata quando si crea un nuovo criterio anti-phishing. Per ottenere risultati ottimali, lasciare l’opzione **attiva**.
  - **Aggiungere mittenti e domini attendibili:** Per questo esempio, non definire sostituzioni.
- Dopo aver esaminato le impostazioni, selezionare **Crea questo criterio** o **Salva**, come appropriato.

Per ulteriori informazioni, vedere [Criteri anti-phishing in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
