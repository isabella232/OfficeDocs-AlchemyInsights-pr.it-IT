---
title: Inviare un messaggio di posta elettronica fornendo l'ID del messaggio di rete
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
ms.openlocfilehash: 1a6f9815a36cc267a815ff9757d713afed5d95aec4f7c537135c88cadf26cc51
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929921"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Inviare un messaggio di posta elettronica fornendo l'ID del messaggio di rete

1. Nel riquadro **a comparsa Nuovo invio** selezionare E-mail e ID messaggio di **rete.** 
2. Seguire questa procedura per trovare l'ID messaggio per un messaggio di posta elettronica in Outlook:
    1. Fare doppio clic sul messaggio di posta elettronica per aprirlo.
    1. Selezionare **Proprietà**  >  **file**.
    1. Aprire Blocco note o un documento di Word vuoto e quindi copiare e incollare il contenuto trovato nella casella Intestazioni **Internet** nel documento aperto per una migliore visibilità.
    1. Individuare il **campo X-MS-Exchange-Organization-Network-Message-Id.** Il valore dopo **: è** l'ID necessario per l'invio.
3. In **Destinatari**, se il messaggio di posta elettronica è atterrato nella cartella posta indesiderata per tutti i destinatari del messaggio di posta elettronica, scegliere **Seleziona tutto**. In caso contrario, selezionare solo l'utente che ha segnalato il problema.
4. In **Motivo dell'invio,** se si seleziona Deve essere **bloccato,** specificare se il messaggio deve essere stato bloccato come **Posta** indesiderata, **Phishing** o **Malware** e quindi selezionare **Invia.**

Per ulteriori informazioni, vedere Come inviare a Microsoft la posta indesiderata sospetta, il phish, gli URL e [i file per l'analisi.](https://go.microsoft.com/fwlink/?linkid=2101479)
