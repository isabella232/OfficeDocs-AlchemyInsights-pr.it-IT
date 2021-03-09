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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552421"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Esempio di criterio anti-phishing di Microsoft Defender per Office 365

Queste impostazioni abilitano un criterio *denominato Dominio e CEO.* Questo criterio fornisce la protezione sia dell'utente che del dominio dalla rappresentazione e quindi applica il criterio a tutti i messaggi di posta elettronica ricevuti dagli utenti all'interno del dominio. Innanzitutto, aggiungere le informazioni seguenti per creare il criterio:

- **Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.
  **Applicato a**: Selezionare **il dominio del destinatario.** In **Una di queste opzioni** selezionare **Scegli** e quindi selezionare un dominio. Selezionare **+ Aggiungi**. Selezionare la casella di controllo accanto al nome del dominio nell'elenco , ad esempio *contoso.com*), quindi selezionare **Aggiungi**. Scegliere **Fatto**.
- Dopo aver creato il criterio, è possibile ottimizzare il criterio utilizzando le opzioni seguenti:
  - **Aggiungere utenti da proteggere:** Per questo esempio, aggiungere almeno l'indirizzo di posta elettronica del CEO.
  - **Aggiungere domini da proteggere:** aggiungere il dominio dell'organizzazione che include l'ufficio del CEO.
  - **Choose actions**: For **If email is sent by an impersonated user,** select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*). Per **Se la posta elettronica viene inviata da un dominio rappresentato,** selezionare **Metti in quarantena il messaggio.**
  - **Intelligence per le** cassette postali: per impostazione predefinita, questa opzione è selezionata quando si crea un nuovo criterio anti-phishing. Per ottenere risultati ottimali, lasciare l’opzione **attiva**.
  - **Aggiungere domini e mittenti attendibili:** Per questo esempio, non definire sostituzioni.
- Dopo aver esaminato le impostazioni, selezionare Crea **questo criterio** o **Salva**, in base alle esigenze.

Per ulteriori informazioni, vedere [Criteri anti-phishing in Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
