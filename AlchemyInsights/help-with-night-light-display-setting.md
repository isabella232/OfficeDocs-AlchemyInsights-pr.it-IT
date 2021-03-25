---
title: Guida per l’impostazione della luce notturna
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123080"
---
# <a name="help-with-the-night-light-display-setting"></a>Guida per l’impostazione della luce notturna

Per altre informazioni sulle impostazioni della luce notturna, [impostare l'orario notturno in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

Se le opzioni per la luce notturna sono disattivate in Impostazioni, controllare il driver video: 

1. Fare clic sulla casella di ricerca della barra delle applicazioni e digitare **Gestione dispositivi**, quindi selezionare **Gestione dispositivi** nei risultati della ricerca.
1. Espandere **schede video**. 

Purtroppo, la caratteristica Luce notturna non è disponibile se il dispositivo usa un driver DisplayLink o un driver video Basic.

La caratteristica Luce notturna usa la recente tecnologia di grafica, quindi potrebbe essere necessario aggiornare il driver video:  

- Controllare la disponibilità di aggiornamenti andando a **Start** > **Impostazioni** > **Aggiornamento e sicurezza** > **Windows Update** > **Controlla aggiornamenti**.  

OPPURE

- Visitare il sito Web del supporto del produttore hardware per scaricare e installare manualmente i driver video più recenti.

## <a name="reset-night-light-in-the-registry"></a>Ripristinare la luce notturna nel Registro di sistema

Se l'aggiornamento del driver video non funziona, potrebbe essere necessario ripristinare la luce notturna nel Registro di sistema.  

**Attenzione:** questa procedura di risoluzione dei problemi è consigliata solo per gli utenti avanzati. L'errata modifica del Registro di sistema può causare seri problemi. Per una maggiore protezione, eseguire un backup del Registro di sistema prima di modificarlo in modo da poterlo ripristinare in cso di problemi.

1. Nella casella di ricerca digitare **regedit** e quindi selezionare **Editor del Registro di sistema** nei risultati della ricerca.

1. Passare alla seguente chiave del Registro di sistema: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Esportare ed eliminare la sottochiave seguente:$$windows.data.bluelightreduction.bluelightreductionstate

1. Esportare ed eliminare la sottochiave seguente:xport and then delete the following subkey:$$windows.data.bluelightreduction.settings

1. Riavviare Windows e verificare se sono disponibili le opzioni per la luce notturna.


