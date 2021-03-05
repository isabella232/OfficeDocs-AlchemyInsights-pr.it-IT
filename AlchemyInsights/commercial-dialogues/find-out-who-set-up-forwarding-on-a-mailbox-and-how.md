---
title: Scoprire chi ha configurato l'inoltro su una cassetta postale e come
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464616"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Scoprire chi ha configurato l'inoltro su una cassetta postale e come

Se l'inoltro esterno è stato impostato su una cassetta postale, l'attività viene verificata come parte del cmdlet Set-Mailbox. Ecco come trovare l'attività nel log di controllo:

1. Passare al Centro sicurezza e conformità di [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selezionare **Ricerca log** di >  **controllo**.
    > [!NOTE]
    > Se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora. Se questa funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.
1. Verificare che il **campo Attività** sia impostato su Mostra risultati per tutte **le attività** (impostazione predefinita). Specificare l'intervallo di date. Non è necessario specificare un nome utente.
1. Selezionare **Cerca.** Le attività vengono visualizzate in **Risultati.**
1. Selezionare **Risultati filtro,** quindi immettere **Set-mailbox** nel **campo Filtro** attività. In questo modo vengono **restituite tutte le attività Set-Mailbox.**
1. Per visualizzare i dettagli, selezionare un'attività e quindi **selezionare Altre informazioni.** In **Parametri** è possibile visualizzare l'indirizzo di posta elettronica di inoltro impostato nella cassetta postale. **L'ID utente** rappresenta l'utente che ha configurato l'inoltro esterno nella cassetta postale.
Per ulteriori informazioni, vedere Eseguire una ricerca nel log di controllo di [Office 365 per risolvere i problemi relativi agli scenari comuni.](https://go.microsoft.com/fwlink/?linkid=2103944)