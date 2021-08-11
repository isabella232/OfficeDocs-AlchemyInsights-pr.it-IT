---
title: Impostazioni di avvio in Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909830"
---
# <a name="startup-settings-in-windows-10"></a>Impostazioni di avvio in Windows 10

**Modificare le app eseguite automaticamente all'avvio**

1. Vai a [Impostazioni > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).

2. Assicurati che tutte le app che vuoi eseguire all'avvio siano **attivate.**

**Aggiungere un'app da eseguire automaticamente all'avvio**

1. Tocca o fai **clic sul pulsante Start** e trova l'app che vuoi eseguire all'avvio.

2. Fai clic con il pulsante destro del mouse sull'app, fai clic **su Altro** e quindi su Apri **percorso file.** Verrà aperto il percorso in cui viene salvato il collegamento all'app. Se non è disponibile alcuna opzione per Apri percorso file, significa che l'app non può essere eseguita all'avvio.

3. Con il percorso del file aperto, premere **il Windows logo + R,** digitare **shell:startup,** quindi fare clic su **OK.** Verrà aperta la cartella Esecuzione automatica.

4. Copia e incolla il collegamento all'app dal percorso del file alla cartella Startup.

**Opzioni di avvio avanzate (tra cui Cassaforte, impostazioni UEFI e avvio da un altro dispositivo)**

1. Salva il lavoro e chiudi tutti i documenti aperti, poiché questi passaggi riavvieranno il PC.

2. Passare a [Impostazioni > aggiornamento & sicurezza > ripristino](ms-settings:recovery?activationSource=GetHelp).

3. In **Avvio avanzato** fare clic su **Riavvia ora.** 

4. Dopo il riavvio del PC nella schermata Scegliere un'opzione:

    - Per eseguire l'avvio da un dispositivo come un'unità USB, fai clic **su Usa un dispositivo.**

    - Per immettere le impostazioni UEFI (a volte denominate configurazione del BIOS), fare clic su Risoluzione dei problemi > opzioni avanzate **> firmware UEFI Impostazioni**. 

    - Per accedere Cassaforte modalità di avvio avanzata o modificare le impostazioni di avvio avanzate, fare clic su Risoluzione dei problemi > opzioni avanzate **> avvio Impostazioni** e quindi fare clic su **Riavvia**. Potrebbe essere richiesto di immettere la chiave di [ripristino di BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Dopo il riavvio del PC, fai clic sull'impostazione di avvio che vuoi usare.