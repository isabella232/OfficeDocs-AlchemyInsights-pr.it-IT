---
title: Crittografare automaticamente determinati messaggi di posta elettronica di Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510216"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Crittografare automaticamente determinati messaggi di posta elettronica di Office 365

È possibile crittografare automaticamente i messaggi inviati dagli utenti a determinate persone o organizzazioni esterne. A tale scopo, eseguire la procedura seguente:

1. [Dall'interfaccia di amministrazione di Exchange,](https://outlook.office365.com/ecp/)scegliere le regole del flusso > **posta.** 
2. Fare clic **sull'icona Nuovo (+)** e quindi su Applica crittografia dei messaggi di **Office 365 e** protezione dei diritti ai messaggi.
3. In **Nome** immettere un nome per la regola, ad esempio Crittografa i *messaggi inviati a DrToniRamos@gmail.com.*
4. In **Applica questa regola se**, scegliere Il **destinatario > è questa persona.** 
5. Nella finestra **Seleziona membri** selezionare il nome della persona a cui si desidera applicare la regola di crittografia e quindi fare clic su **Aggiungi.** 
6. Al termine dell'aggiunta degli utenti, fare clic su **OK.**
7. Accanto al campo **Fare clic** su **Seleziona.** 
8. Nel menu **a discesa del** modello RMS selezionare **Crittografa** e quindi fare clic su **OK.** Se questa opzione non è visualizzata, significa che il piano non include la crittografia automatica. Ma puoi aggiungerlo!)
9. Scegli una selezione facoltativa (da un elenco di selezioni facoltative che puoi effettuare a questo punto, molte delle quali possono essere lasciata con l'impostazione predefinita per semplicità).
10. Fare clic su **Salva**.

> [!IMPORTANT]
> È sempre possibile tornare indietro e modificare questa regola in un secondo momento.

Per ulteriori informazioni sulla creazione di regole per la crittografia, vedere Definire le regole del flusso di posta per crittografare i messaggi di posta [elettronica in Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

