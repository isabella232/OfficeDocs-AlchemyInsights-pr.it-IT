---
title: Crittografare automaticamente determinati messaggi di posta elettronica da Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50510224"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Crittografare automaticamente determinati messaggi di posta elettronica da Office 365

1. [Nell'interfaccia di amministrazione di Exchange](https://outlook.office365.com/ecp/)scegliere le regole del flusso > **posta.** 
2. Fare clic **sull'icona Nuovo (+)** e quindi su Applica crittografia dei messaggi di **Office 365 e** protezione dei diritti ai messaggi.
3. In **Nome** immettere un nome per la regola, ad esempio *Crittografa tutti i messaggi.*
4. In **Applica questa regola se**, scegliere **[Applica a tutti i messaggi]**. 
5. Accanto al campo **Fare clic** su **Seleziona.** 
6. Nel menu **a discesa del** modello RMS selezionare **Crittografa** e quindi fare clic su **OK.** Se questa opzione non è visualizzata, significa che il piano non include la crittografia automatica. Ma puoi aggiungerlo!)
7. Selezionare la **casella di controllo Controlla questa regola con livello di gravità** e quindi selezionare il livello desiderato. Se l'azienda ha obblighi contrattuali per inviare tutti i messaggi di posta elettronica crittografati, ti consigliamo di impostare il livello su **Alto.**
8. In **Scegliere un modello per la regola fare** clic su **Applica.** 
9. Scegli una selezione facoltativa (da un elenco di selezioni facoltative che puoi effettuare a questo punto, molte delle quali possono essere lasciata con l'impostazione predefinita per semplicità).
10. Fare clic su **Salva**.

> [!IMPORTANT]
> È sempre possibile tornare indietro e modificare questa regola in un secondo momento.

Per ulteriori informazioni sulla creazione di regole per la crittografia, vedere Definire le regole del flusso di posta per crittografare i messaggi di posta [elettronica in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

