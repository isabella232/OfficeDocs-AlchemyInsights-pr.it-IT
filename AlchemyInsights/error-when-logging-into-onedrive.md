---
title: 0x8004de40 errore durante l'avvio di OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813656"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 errore durante l'avvio di OneDrive

Se viene visualizzato un messaggio di **0x8004de40** durante l'accesso a OneDrive, riavviare il computer mentre si è connessi al dominio dell'istituto di istruzione o dell'istituto di istruzione. Se viene visualizzato questo errore dopo il riavvio, provare a eseguire questa operazione mentre si è connessi al dominio dell'istituto di istruzione o dell'istituto di istruzione:

1. Fare clic sul pulsante Start e digitare **cmd** o **prompt** dei comandi nella casella di ricerca, fare clic con il pulsante destro del mouse sull'app del prompt dei comandi e scegliere **Esegui come amministratore.** Se viene richiesta una password di amministratore o una conferma, digitare la password o fare clic su **Consenti**.  

2. Nella finestra del prompt dei comandi digitare **dsregcmd /leave**  e attendere il completamento del comando. Digitare **quindi dsregcmd /join e** attendere il completamento del comando.
3. Riavviare il computer.
