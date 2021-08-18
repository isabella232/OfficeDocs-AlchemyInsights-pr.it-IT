---
title: Identificare l'inoltro esterno della posta elettronica nelle cassette postali nei registri di controllo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331163"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificare quando l'inoltro di posta elettronica esterno è configurato sulle cassette postali

Quando un Microsoft 365 utente configura l'inoltro esterno della posta elettronica su una cassetta postale, l'attività viene verificata come parte del cmdlet **Set-Mailbox.** È possibile visualizzare l'attività utilizzando la ricerca nei log di controllo. Ecco come farlo.

1. Eseguire uno dei seguenti passaggi:
   - Nel Centro conformità Microsoft 365 in <https://compliance.microsoft.com>, passare a **Soluzioni** \> **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://compliance.microsoft.com/auditlogsearch>.
   - Nel portale di Microsoft 365 Defender in <https://security.microsoft.com>, passare ad **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://sip.security.microsoft.com/auditlogsearch>.

2. Alla pagina **Audit**, verificare che la scheda **Cerca** sia selezionata e configurare le seguenti impostazioni:
   - Selezionare l'intervallo di data/ora nelle **caselle Inizio** **e** Fine.
   - Verificare che **la casella** Attività contenga Mostra risultati per tutte **le attività.**

3. Una volta terminato, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova pagina **Ricerca audit**.

4. Nei risultati, fare clic su **Filtra risultati** e digitare **Set-Mailbox** nella casella filtro attività.

5. Selezionare un record di audit nei risultati. Nel riquadro **a comparsa** Dettagli fare clic su **Altre informazioni.** È necessario esaminare i dettagli di ogni record di controllo per determinare se l'attività è correlata all'inoltro della posta elettronica.

   - **ObjectId**: Valore alias della cassetta postale modificata.
   - **Parametri**: _ForwardingSmtpAddress_ indica l'indirizzo di posta elettronica di destinazione.
   - **UserId**: l'utente che ha configurato l'inoltro della posta elettronica sulla cassetta postale nel **campo ObjectId.**

Per ulteriori informazioni, vedere [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
