---
title: Sincronizzazione dei contatti di Teams
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
- "9004610"
- "11540"
ms.openlocfilehash: efc1f29c6e2f76d763f2f8102db7e9f6afb1f1be
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327337"
---
# <a name="teams-contacts-sync"></a>Sincronizzazione dei contatti di Teams

Teams usa i contatti presenti in Active Directory dell'organizzazione e i contatti aggiunti alla cartella predefinita di Outlook dell'utente. Se i contatti non vengono visualizzati in Microsoft Teams, prova quanto segue:

**Nota:** se le informazioni di uno o più contatti sono state aggiornate di recente, la sincronizzazione dei contatti può richiedere fino a 48 ore.

1. Esci da Teams e riavvia. Controlla se i contatti vengono visualizzati.
1. Cancella la cache di Teams:
    1. Passa a **%appdata%\Microsoft\Teams**.
    1. Elimina i contenuti della cartella.
    1. Riavvia il computer e avvia Teams.
1. Se il contatto è in Outlook, assicurati di aggiungerlo nell'elenco contatti. In Outlook, dalla barra degli indirizzo, seleziona **File**, quindi **Aggiungi a contatti**.
1. Verifica che la cassetta postale di Exchange dell'utente sia ospitata online (non in locale). Per altre informazioni, vedere [Interazione tra Exchange e Microsoft Teams](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
1. Assicurati che il numero di telefono del contatto sia aggiunto alle informazioni di contatto.
1. Cerca il messaggio di posta elettronica del contatto nella barra di ricerca. I contatti recuperati vengono sincronizzati con l'elenco Contatti.
