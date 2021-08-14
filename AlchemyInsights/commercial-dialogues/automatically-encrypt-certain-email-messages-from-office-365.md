---
title: Crittografare automaticamente alcuni messaggi di posta elettronica da Office 365
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
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988839"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Crittografare automaticamente alcuni messaggi di posta elettronica da Office 365

1. [Nell'Exchange di amministrazione scegliere](https://outlook.office365.com/ecp/)flusso di posta > **regole.** 
2. Fare clic **sull'icona Nuovo (+)** e quindi su Applica Office 365 Message Encryption **protezione dei diritti ai messaggi**.
3. In **Nome** immettere un nome per la regola, ad esempio *Crittografa tutti i messaggi.*
4. In **Applica questa regola se** scegliere **[Applica a tutti i messaggi]**. 
5. Accanto al campo **Eseguire le operazioni** seguenti, fare clic su Seleziona **uno**. 
6. Nel menu **a discesa** Modello RMS selezionare Crittografa e quindi fare clic su **OK.**  Se questa opzione non è disponibile, significa che il piano non include la crittografia automatica. Ma è possibile aggiungerlo!)
7. Selezionare la **casella di controllo Controlla questa regola con livello di gravità** e quindi selezionare il livello desiderato. Se la tua azienda ha obblighi contrattuali per inviare tutti i messaggi di posta elettronica crittografati, ti consiglio di impostare il livello su **High**.
8. In **Scegliere un modello per questa regola fare** clic su **Applica.** 
9. Scegliere qualsiasi selezione facoltativa (da un elenco di selezioni facoltative che è possibile effettuare a questo punto, molte delle quali possono essere lasciati con l'impostazione predefinita per semplicità).
10. Fare clic su **Salva**.

> [!IMPORTANT]
> È sempre possibile tornare e modificare questa regola in un secondo momento.

Per ulteriori informazioni sulla creazione di regole per la crittografia, vedere [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

