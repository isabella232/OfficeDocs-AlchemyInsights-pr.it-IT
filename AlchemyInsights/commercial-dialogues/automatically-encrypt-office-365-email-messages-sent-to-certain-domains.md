---
title: Crittografare automaticamente Office 365 messaggi di posta elettronica inviati a determinati domini
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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082190"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Crittografare automaticamente Office 365 messaggi di posta elettronica inviati a determinati domini

1. [Nell'Exchange di amministrazione scegliere](https://outlook.office365.com/ecp/)flusso di posta > **regole.** 
2. Fare clic **sull'icona Nuovo (+)** e quindi su Applica Office 365 Message Encryption **protezione dei diritti ai messaggi**.
3. In **Nome** immettere un nome per la regola, ad esempio *Crittografa* i messaggi inviati a contoso.com .
4. In **Applica questa regola se** scegliere Il **destinatario > dominio è**. 
5. Immettere il nome del dominio, ad esempio **contoso.com**.
6. Fare clic **sull'icona Aggiungi (+)** e quindi su **OK.**
7. Accanto al campo **Eseguire le operazioni** seguenti, fare clic su Seleziona **uno**. 
8. Nel menu **a discesa** Modello RMS selezionare Crittografa e quindi fare clic su **OK.**  Se questa opzione non è disponibile, significa che il piano non include la crittografia automatica. Ma è possibile aggiungerlo!)
9. Scegliere qualsiasi selezione facoltativa (da un elenco di selezioni facoltative che è possibile effettuare a questo punto, molte delle quali possono essere lasciati con l'impostazione predefinita per semplicità).
10. Fare clic su **Salva**.

> [!IMPORTANT]
> È sempre possibile tornare e modificare questa regola in un secondo momento.

Per ulteriori informazioni sulla creazione di regole per la crittografia, vedere [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)