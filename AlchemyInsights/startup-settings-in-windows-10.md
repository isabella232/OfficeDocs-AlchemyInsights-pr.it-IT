---
title: Impostazioni di avvio in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751139"
---
# <a name="startup-settings-in-windows-10"></a>Impostazioni di avvio in Windows 10

**Modificare le app eseguite automaticamente all'avvio**

1. Andare a [impostazioni > > di avvio delle app](ms-settings:startupapps?activationSource=GetHelp).

2. Verificare che l'applicazione che si desidera eseguire all'avvio sia attivata **.**

**Aggiungere un'app per l'esecuzione automatica all'avvio**

1. Fare clic o toccare **Avvia** e trovare l'app che si desidera eseguire all'avvio.

2. Fare clic con il pulsante destro del mouse sull'app, scegliere **altro**e quindi fare clic su **Apri percorso file**. Verrà aperta la posizione in cui viene salvato il collegamento all'app. Se non è disponibile alcuna opzione per il percorso del file aperto, significa che l'app non può essere eseguita all'avvio.

3. Con il percorso del file aperto, premere il **tasto logo Windows + R**, digitare **Shell: Startup**e quindi fare clic su **OK**. Verrà aperta la cartella di avvio.

4. Copiare e incollare il collegamento all'app dal percorso del file alla cartella di avvio.

**Opzioni di avvio avanzate (tra cui modalità provvisoria, impostazioni UEFI e avvio da un altro dispositivo)**

1. Salvare il lavoro e chiudere tutti i documenti aperti, poiché questi passaggi ricominceranno il PC.

2. Passare a [impostazioni > aggiornamento & sicurezza > ripristino](ms-settings:recovery?activationSource=GetHelp).

3. In **avvio avanzato**fare clic su **Riavvia**. 

4. Dopo aver riavviato il PC nella schermata Scegli un'opzione:

    - Per eseguire l'avvio da un dispositivo come un'unità USB, fare clic su **USA dispositivo**.

    - Per immettere le impostazioni UEFI (a volte chiamata configurazione del BIOS), fare clic su **risoluzione dei problemi > opzioni avanzate > impostazioni del firmware UEFI**. 

    - Per attivare la modalità provvisoria o modificare le impostazioni di avvio avanzato, fare clic su **risoluzione dei problemi > opzioni avanzate > impostazioni di avvio**, quindi fare clic su **Riavvia** Potrebbe essere richiesto di immettere la [chiave di ripristino di BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key). Dopo aver riavviato il PC, fare clic sull'impostazione di avvio che si desidera utilizzare.