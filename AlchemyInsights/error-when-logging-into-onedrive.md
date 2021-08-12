---
title: 0x8004de40 errore durante l'avvio OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946583"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 errore durante l'avvio OneDrive

Se viene visualizzato un messaggio di **0x8004de40** durante l'accesso OneDrive, riavviare il computer mentre si è connessi al dominio dell'istituto di istruzione o dell'istituto di istruzione. Se viene visualizzato questo errore dopo il riavvio, provare a eseguire questa operazione mentre si è connessi al dominio dell'istituto di istruzione o dell'istituto di istruzione:

1. Fare clic sul pulsante Start e digitare **cmd** o **prompt** dei comandi nella casella di ricerca, fare clic con il pulsante destro del mouse sull'app del prompt dei comandi e scegliere **Esegui come amministratore.** Se viene richiesta una password di amministratore o una conferma, digitare la password o fare clic su **Consenti**.  

2. Nella finestra del prompt dei comandi digitare **dsregcmd /leave**  e attendere il completamento del comando. Digitare **quindi dsregcmd /join e** attendere il completamento del comando.
3. Riavviare il computer.
