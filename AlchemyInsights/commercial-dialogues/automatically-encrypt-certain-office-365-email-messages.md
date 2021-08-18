---
title: Crittografare automaticamente alcuni Office 365 di posta elettronica
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: b15a72ced4921b3df1b7105837592781188a2a25
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327978"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Crittografare automaticamente alcuni Office 365 di posta elettronica

È possibile crittografare automaticamente i messaggi inviati dagli utenti a determinate persone o organizzazioni esterne. A tale scopo, eseguire la procedura seguente:

1. [Nell'Exchange di amministrazione scegliere](https://outlook.office365.com/ecp/)flusso di posta > **regole.** 
2. Fare clic **sull'icona Nuovo (+)** e quindi su Applica Office 365 Message Encryption **protezione dei diritti ai messaggi**.
3. In **Nome** immettere un nome per la regola, ad esempio *Crittografa* i messaggi inviati a DrToniRamos@gmail.com .
4. In **Applica questa regola se**, scegliere Il **destinatario > è questa persona.** 
5. Nella finestra **Seleziona membri** selezionare il nome della persona a cui si desidera applicare la regola di crittografia e quindi fare clic su **Aggiungi.** 
6. Al termine dell'aggiunta degli utenti, fare clic su **OK.**
7. Accanto al campo **Eseguire le operazioni** seguenti, fare clic su Seleziona **uno**. 
8. Nel menu **a discesa** Modello RMS selezionare Crittografa e quindi fare clic su **OK.**  Se questa opzione non è disponibile, significa che il piano non include la crittografia automatica. Ma è possibile aggiungerlo!)
9. Scegliere qualsiasi selezione facoltativa (da un elenco di selezioni facoltative che è possibile effettuare a questo punto, molte delle quali possono essere lasciati con l'impostazione predefinita per semplicità).
10. Fare clic su **Salva**.

**Importante:** è sempre possibile tornare e modificare questa regola in un secondo momento.

Per ulteriori informazioni sulla creazione di regole per la crittografia, vedere [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

