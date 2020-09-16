---
title: Icona della batteria o dell'alimentazione non presente in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 10213843f8ec5ceeaa191d3373406d767f2bea3c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771545"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Icona della batteria o dell'alimentazione non presente in Windows 10

Se il dispositivo Windows 10 è dotato di una batteria (ad es. portatile o tablet o PC connesso a un USP tramite USB), in genere l'icona della batteria/alimentazione è visibile nella barra delle applicazioni accanto all'orologio, ad esempio:

![Icona della batteria](media/battery-icon.png)

Se tale icona non è visibile, è possibile che sia nascosta:

1. Passare a **[Impostazioni > Personalizzazione > Barra delle applicazioni](ms-settings:taskbar?activationSource=GetHelp)**.

2. Nell'area Notifica fare clic su **Seleziona le icone da visualizzare sulla barra delle applicazioni**.

3. Trovare quindi l'elemento **Alimentazione** nell'elenco e spostare l'impostazione su **Attivato**.

    ![Mostrare l'icona dell'alimentazione nella barra delle applicazioni](media/power-icon-on.png)

**Risoluzione dei problemi**

Se sono state seguite le istruzioni riportate sopra e l'interruttore **Alimentazione** è disattivato o non è visibile, nella casella di ricerca della barra delle applicazioni digitare **gestione dispositivi**, quindi selezionare **Gestione dispositivi** nell'elenco dei risultati. In **Batterie** fare clic con il pulsante destro sulla batteria del dispositivo, fare clic su **Disabilita**, quindi su **Sì**. Attendere qualche secondo, quindi fare clic con il pulsante destro sulla batteria e fare clic su **Abilita**. Riavviare il dispositivo.

Se sono state seguite le istruzioni riportate sopra, ma l'icona della batteria non viene visualizzata nella barra delle applicazioni, nella casella di ricerca della barra delle applicazioni digitare **gestione attività**, quindi fare clic su **Gestione attività** nell'elenco dei risultati. Nella scheda **Processi** sotto **Nome** fare clic con il pulsante destro su **Explorer**, quindi fare clic su **Riavvia**.
