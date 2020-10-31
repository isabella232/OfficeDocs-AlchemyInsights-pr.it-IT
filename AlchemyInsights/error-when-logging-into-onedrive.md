---
title: errore 0x8004de40 durante l'avvio di OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815993"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>errore 0x8004de40 durante l'avvio di OneDrive

Se viene visualizzato un messaggio di errore **0x8004de40** durante l'accesso a OneDrive, riavviare il computer quando si è connessi al dominio di lavoro o della scuola. Se si riceve questo errore dopo il riavvio, provare a eseguire questa operazione quando si è connessi al dominio di lavoro o della scuola:

1. Fare clic sul pulsante Start e digitare **cmd** o **prompt dei comandi**  nella casella di ricerca, fare clic con il pulsante destro del mouse sull'app del prompt dei comandi e scegliere  **Esegui come amministratore** . Se viene richiesta una password di amministratore o per una conferma, digitare la password oppure fare clic su **Consenti** .  

2. Nella finestra del prompt dei comandi digitare **dsregcmd/Leave**  e attendere il completamento del comando. Digitare **dsregcmd/join** e attendere il completamento del comando.
3. Riavviare il computer.
