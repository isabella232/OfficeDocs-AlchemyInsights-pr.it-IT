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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317812"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Individuare chi ha configurato l'inoltro su una cassetta postale e come

Se l'inoltro esterno è stato impostato su una cassetta postale, l'attività viene verificata come parte del cmdlet **Set-Mailbox.** Ecco come trovare l'attività nel log di controllo:

1. Eseguire una delle operazioni seguenti:
   - Nel Centro conformità Microsoft 365 in <https://compliance.microsoft.com>, passare a **Soluzioni** \> **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://compliance.microsoft.com/auditlogsearch>.
   - Nel portale di Microsoft 365 Defender in <https://security.microsoft.com>, passare ad **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://security.microsoft.com/auditlogsearch>.

   **Nota:** se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora. Se questa funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.

2. Alla pagina **Audit**, verificare che la scheda **Cerca** sia selezionata e configurare le seguenti impostazioni:
   - Selezionare l'intervallo di data/ora nelle **caselle Inizio** **e** Fine.
   - Verificare che **la casella** Attività contenga Mostra risultati per tutte **le attività.**

3. Una volta terminato, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova pagina **Ricerca audit**.

4. Nei risultati, fare clic sulla **colonna Attività** per ordinare i risultati e cercare **Voci Set-Mailbox.**

5. Selezionare un'attività nei risultati per aprire il riquadro a comparsa dei dettagli. È necessario esaminare i dettagli di ogni record di controllo per determinare se l'attività è correlata all'inoltro della posta elettronica:
   - **ObjectId**: Valore alias della cassetta postale modificata.
   - **Parametri**: _ForwardingSmtpAddress_ indica l'indirizzo di posta elettronica di destinazione.
   - **UserId**: l'utente che ha configurato l'inoltro della posta elettronica sulla cassetta postale nel **campo ObjectId.**

Per ulteriori informazioni, vedere [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
