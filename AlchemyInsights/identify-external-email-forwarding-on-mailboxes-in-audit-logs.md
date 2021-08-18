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
ms.openlocfilehash: 2af731bc9a1e28e2db7c6662041b930e1b05be4c3bf8340784d9ab87101c44af
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899888"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identificare quando l'inoltro di posta elettronica esterno è configurato sulle cassette postali

Quando un Microsoft 365 utente configura l'inoltro esterno della posta elettronica su una cassetta postale, l'attività viene verificata come parte del cmdlet **Set-Mailbox.** È possibile visualizzare l'attività utilizzando la ricerca nei log di controllo. Ecco come farlo.

1. Esegui uno dei seguenti passaggi:
   - Nella finestra Centro conformità Microsoft 365 <https://compliance.microsoft.com> , passare a **Soluzioni** \> **Controllo**. In caso contrario, per passare direttamente alla **pagina Controllo,** utilizzare <https://compliance.microsoft.com/auditlogsearch> .
   - Nel portale Microsoft 365 Defender <https://security.microsoft.com> all'indirizzo , passare a **Controlla**. In caso contrario, per passare direttamente alla **pagina Controllo,** utilizzare <https://sip.security.microsoft.com/auditlogsearch> .

2. Nella pagina **Controllo** verificare che la scheda **Ricerca** sia selezionata e quindi configurare le impostazioni seguenti:
   - Selezionare l'intervallo di data/ora nelle **caselle Inizio** **e** Fine.
   - Verificare che **la casella** Attività contenga Mostra risultati per tutte **le attività.**

3. Al termine, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova **pagina Di ricerca di** controllo.

4. Nei risultati, fare clic **su Filtra risultati** e digitare **Set-Mailbox** nella casella filtro attività.

5. Selezionare un record di controllo nei risultati. Nel riquadro **a comparsa** Dettagli fare clic su **Altre informazioni.** È necessario esaminare i dettagli di ogni record di controllo per determinare se l'attività è correlata all'inoltro della posta elettronica.

   - **ObjectId**: Valore alias della cassetta postale modificata.
   - **Parametri**: _ForwardingSmtpAddress_ indica l'indirizzo di posta elettronica di destinazione.
   - **UserId**: l'utente che ha configurato l'inoltro della posta elettronica sulla cassetta postale nel **campo ObjectId.**

Per ulteriori informazioni, vedere [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
