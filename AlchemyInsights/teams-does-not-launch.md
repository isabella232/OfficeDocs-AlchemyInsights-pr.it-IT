---
title: Teams non viene avviato
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: ebfabf667092850e5045c56e34e355739944ba44
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329330"
---
# <a name="teams-doesnt-launch"></a>Teams non viene avviato

Se si prova ad aprire Microsoft Teams ma non viene mai avviato, provare a eseguire le operazioni seguenti:

1. Passa a **%appdata%\Microsoft\Teams**.
1. Elimina i contenuti della cartella.
1. Riavviare il computer e provare ad avviare Teams.

Potrebbe essere necessario reinstallare Teams. Per reinstallarlo:

1. Disinstallare Teams mediante il Pannello di controllo.
1. Passare a **%appdata%\Microsoft\Teams\Application Cache**.
1. Eliminare il contenuto della cartella.
1. Passare a **%appdata%\Microsoft\teams\Cache**.
1. Eliminare il contenuto della cartella.
1. Riavviare il computer e quindi scaricare e installare Teams.

Se si vuole eseguire una diagnostica nel tenant per un utente specifico che non può accedere, avviare una nuova ricerca con la parola chiave **TeamsUserUnableToSignIn** e seguire le istruzioni visualizzate.