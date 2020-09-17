---
title: Se si fa doppio clic su un file di Office non è possibile aprirlo
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
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812083"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Se si fa doppio clic su un file di Office non è possibile aprirlo

Dopo aver fatto doppio clic su un file di Office, è possibile che venga visualizzato il programma aperto, ma il file non viene aperto. In alternativa, è possibile che venga visualizzato il messaggio di errore: "si è verificato un problema durante l'invio del comando al programma". Sono presenti molte cause, ma le due soluzioni più comuni sono le seguenti:

- Da Excel, verificare che l'opzione DDE sia deselezionata. È possibile trovare l'opzione creando una nuova cartella di lavoro e quindi scegliendo **File > opzioni > avanzate**. Nella sezione **generale** deselezionare la casella di controllo **Ignora altre applicazioni che utilizzano DDE (Dynamic Data Exchange)**.

- Eseguire un ripristino online per ripristinare le impostazioni predefinite. Fare clic sul pulsante Start di Windows e cercare "pannello di controllo". Aprire il **Pannello di controllo**e passare a **programmi > programmi e funzionalità**. Fare clic con il pulsante destro del mouse su **Microsoft Office [versione]** e scegliere **Change > online Repair**.

Se nessuna di queste soluzioni funziona, è possibile trovare un elenco più completo di soluzioni nell'articolo del supporto, [facendo doppio clic su un file di Office che non riesce ad aprirlo](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).
