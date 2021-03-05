---
title: Trovare l'indirizzo IP nel registro di controllo
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50465002"
---
# <a name="find-the-ip-address-in-audit-log"></a>Trovare l'indirizzo IP nel registro di controllo

1. L'indirizzo IP corrispondente a un'attività eseguita da un utente o da un amministratore viene visualizzato nei registri di controllo. Vengono registrate anche le informazioni sul client. Ecco come identificare l'indirizzo IP:

1. Passare al Centro sicurezza e conformità di [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selezionare **Ricerca log** di  >  **[controllo](https://go.microsoft.com/fwlink/?linkid=2103759)**.
    > [!NOTE]
    > Se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora. Se questa funzionalità non è abilitata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.
1. Se sei interessato a un'attività specifica, selezionala **nell'elenco** Attività. In caso contrario, per impostazione predefinita verranno restituite tutte le attività per l'utente selezionato. Si noti che alcune attività potrebbero non essere disponibili per la selezione **dal** menu Attività. Tuttavia, tali elementi di controllo verranno restituiti se **è selezionata l'opzione** Mostra risultati per tutte le attività (impostazione predefinita).
1. Specificare l'intervallo di date e nel **campo Utenti** selezionare il nome utente dell'utente che si desidera analizzare.
1. Selezionare **Cerca.** Le attività vengono visualizzate in **Risultati.** È possibile visualizzare l'indirizzo IP per ogni attività.
1. Per visualizzare i dettagli, selezionare un'attività e quindi **selezionare Altre informazioni.**

Per ulteriori informazioni, vedere Eseguire una ricerca nel log di controllo di [Office 365 per risolvere i problemi relativi agli scenari comuni.](https://go.microsoft.com/fwlink/?linkid=2103944)