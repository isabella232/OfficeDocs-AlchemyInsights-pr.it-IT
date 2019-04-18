---
title: Identificare l'inoltro di posta elettronica esterno nelle cassette postali nei registri di controllo
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909345"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificare quando l'inoltro di posta elettronica esterno è configurato per le cassette postali

Quando un utente configura l'inoltro di posta elettronica esterno su una cassetta postale, l'attività viene controllata come parte del cmdlet **Set-Mailbox** . È possibile visualizzare l'attività utilizzando la ricerca del registro di controllo nel centro sicurezza & Compliance.

1. Accedere al [centro conformità _AMP_ sicurezza di Office 365](https://protection.office.com/)

2. Fare clic su **ricerca e analisi** e selezionare **Ricerca log di controllo**.

3. Selezionare l'intervallo di date nei campi data di **inizio** e **Data di fine** . Non è necessario specificare un nome utente. Verificare che il campo **attività** sia impostato per **visualizzare i risultati di tutte le attività**.

4. Fare clic su **Cerca**.

Nei risultati, fare clic su **Filtra risultati** e digitare **Set-Mailbox** nella casella filtro attività. Selezionare un record di controllo nei risultati. Nel riquadro a comparsa **Dettagli** , fare clic su **altre informazioni**. Per determinare se l'attività è correlata all'inoltro della posta elettronica, è necessario esaminare i dettagli di ogni record di controllo.

- **ObjectID**: il valore alias della cassetta postale che è stata modificata.

- **Parametri**: _ForwardingSmtpAddress_ indica l'indirizzo di posta elettronica di destinazione.

- **Userid**: l'utente che ha configurato l'inoltro della posta elettronica sulla cassetta postale nel campo **ObjectID** .

Per ulteriori informazioni, vedere [determinare chi ha configurato l'inoltro della posta elettronica per una cassetta postale](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
