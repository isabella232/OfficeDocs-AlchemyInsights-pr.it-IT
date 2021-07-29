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
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630253"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificare quando l'inoltro di posta elettronica esterno è configurato sulle cassette postali

Quando un Microsoft 365 utente configura l'inoltro esterno della posta elettronica su una cassetta postale, l'attività viene verificata come parte del cmdlet **Set-Mailbox.** È possibile visualizzare l'attività usando la ricerca nei log di controllo nel Centro sicurezza & conformità.

1. Accedere al Centro [Microsoft 365 conformità](https://protection.office.com/).

2. Passare alla pagina **ricerca log** di  >  **controllo della** ricerca.

3. Selezionare l'intervallo di date nei **campi Data inizio** e Data **fine.** Non è necessario specificare un nome utente. Verificare che **il campo** Attività sia impostato su Mostra risultati per tutte **le attività.**

4. Fare clic su **Cerca**.

Nei risultati, fare clic **su Filtra risultati** e digitare **Set-Mailbox** nella casella filtro attività. Selezionare un record di controllo nei risultati. Nel riquadro **a comparsa** Dettagli fare clic su **Altre informazioni.** È necessario esaminare i dettagli di ogni record di controllo per determinare se l'attività è correlata all'inoltro della posta elettronica.

- **ObjectId**: valore alias della cassetta postale modificata.

- **Parametri**: _ForwardingSmtpAddress_ indica l'indirizzo di posta elettronica di destinazione.

- **UserId**: l'utente che ha configurato l'inoltro della posta elettronica sulla cassetta postale nel **campo ObjectId.**

Per ulteriori informazioni, vedere [Determining who set up email forwarding for a mailbox](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
