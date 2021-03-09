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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552357"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Inviare un messaggio di posta elettronica fornendo l'ID del messaggio di rete

1. Nel riquadro **a comparsa Nuovo invio** selezionare E-mail e ID messaggio di **rete.** 
2. Seguire questa procedura per trovare l'ID messaggio per un messaggio di posta elettronica in Outlook:
    1. Fare doppio clic sul messaggio di posta elettronica per aprirlo.
    1. Selezionare **Proprietà**  >  **file.**
    1. Aprire blocco note o un documento di Word vuoto e quindi copiare e incollare il contenuto trovato nella casella intestazioni **Internet** nel documento aperto per una maggiore visibilità.
    1. Individuare il **campo X-MS-Exchange-Organization-Network-Message-Id.** Il valore dopo **il parametro :** è l'ID necessario per l'invio.
3. In **Destinatari,** se il messaggio di posta elettronica è atterrato nella cartella posta indesiderata per tutti i destinatari di questo messaggio di posta elettronica, scegliere **Seleziona tutto.** In caso contrario, selezionare solo l'utente che ha segnalato il problema.
4. In **Motivo dell'invio,** se si seleziona Deve essere **bloccato,** specificare se il messaggio deve essere stato bloccato come Posta **indesiderata,** **Phishing** o **Malware,** quindi selezionare **Invia.**

Per ulteriori informazioni, vedere Come inviare posta [indesiderata, phish, URL e file](https://go.microsoft.com/fwlink/?linkid=2101479)sospetti a Microsoft per l'analisi.
