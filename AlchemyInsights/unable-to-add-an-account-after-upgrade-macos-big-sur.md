---
title: Impossibile aggiungere un account dopo l'aggiornamento a macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475128"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Impossibile aggiungere un account dopo l'aggiornamento a macOS 11.6 Big Sur

Dopo l'aggiornamento a macOS 11.6, il proprio OneDrive per l'account aziendale o dell'istituto di istruzione o l'account personale di OneDrive potrebbe non essere visualizzato nell'elenco degli account, in più potrebbe non essere possibile accedere a un secondo account dall'app.

È stata sviluppata una correzione per questo problema. Prima di tutto, determina se sta usando la versione autonoma o dell'App Store di OneDrive:

- Seleziona il cloud OneDrive nella barra dei menu > **Guida & Impostazioni**  >  **Preferenze**  >  **Informazioni**. Se il numero di versione non include **(Autonomo),** hai la versione del prodotto dell'App Store.

Se si usa la versione autonoma di OneDrive, riavvia il computer: OneDrive si aggiorna automaticamente a una versione in cui questo problema è stato risolto. Se vuoi installare manualmente la versione, scarica questo [file di.zip](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip),decomprimi il file e copia l'app OneDrive nella cartella Applicazioni (sostituendo l'app OneDrive esistente).

Se stai usando la versione dell'App Store, valuta la possibilità di installare la versione autonoma di OneDrive. Questa versione funziona allo stesso modo della versione dell'App Store, ma consente a Microsoft di offrire agli utenti gli aggiornamenti più rapidamente e di connetterli a una versione che include la correzione per questo problema.

1. Scarica la versione autonoma di [OneDrive che include la correzione](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip).
2. Decomprimi il file e copia l OneDrive app nella cartella Applicazioni (sostituendo l'app OneDrive esistente).

Se devi usare la versione dell'App Store, attendi che l'App Store rilasci una versione dell'app che include la correzione. Purtroppo, Microsoft non può comunicare una data stimata per il rilascio di una versione fissa dall'App Store.


