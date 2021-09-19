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
ms.openlocfilehash: a8176de71a1f67004e790a3a98943402a240f656
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446744"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Impossibile aggiungere un account dopo l'aggiornamento a macOS 11.6 Big Sur

Dopo l'aggiornamento a macOS 11.6, il proprio OneDrive per l'account aziendale o dell'istituto di istruzione o l'account personale di OneDrive potrebbe non essere visualizzato nell'elenco degli account, in più potrebbe non essere possibile accedere a un secondo account dall'app.

Si tratta di un nuovo problema relativo all'aggiornamento a macOS 11.6. Finché il problema non verrà risolto, sarà possibile accedere al contenuto di OneDrive dal Web o dal dispositivo mobile. Microsoft sta collaborando attivamente con Apple per ripristinare la funzionalità di OneDrive.

È anche possibile avviare manualmente l'istanza di OneDrive mancante usando Terminale. 

**Nota**: questa soluzione alternativa funziona solo OneDrive viene riavviato del computer (con un riavvio del computer o un aggiornamento dell’app OneDrive).

Se l'istanza mancante è l'account personale, aprire Terminale e immettere:

`open "/Applications/OneDrive.app" --new --args /client=Personal`

Se l'istanza mancante è l'account aziendale o dell'istituto di istruzione, aprire Terminale e immettere:

`open "/Applications/OneDrive.app" --new --args /client=Business1`

