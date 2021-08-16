---
title: Individuare chi ha configurato l'inoltro su una cassetta postale e come
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988207"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Individuare chi ha configurato l'inoltro su una cassetta postale e come

Se l'inoltro esterno è stato impostato su una cassetta postale, l'attività viene verificata come parte del cmdlet Set-Mailbox. Ecco come trovare l'attività nel log di controllo:

1. Passare al Centro [Office 365 sicurezza & conformità](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Selezionare **Ricerca** >  **log di controllo ricerca**.
    > [!NOTE]
    > Se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora. Se questa funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.
1. Verificare che il **campo** Attività sia impostato su **Mostra risultati per tutte le attività** (impostazione predefinita). Specificare l'intervallo di date. Non è necessario specificare un nome utente.
1. Selezionare **Cerca**. Le attività vengono visualizzate in **Risultati**.
1. Selezionare **Filtra risultati** e quindi immettere **Set-mailbox** nel **campo Filtro** attività. In questo modo vengono **restituite tutte le attività set-mailbox.**
1. Per visualizzare i dettagli, selezionare un'attività e quindi **selezionare Altre informazioni.** In **Parametri** è possibile visualizzare l'indirizzo di posta elettronica di inoltro impostato sulla cassetta postale. UserID **rappresenta** l'utente che ha configurato l'inoltro esterno nella cassetta postale.
Per ulteriori informazioni, vedere [Search the Office 365 audit log to troubleshoot common scenarios.](https://go.microsoft.com/fwlink/?linkid=2103944)