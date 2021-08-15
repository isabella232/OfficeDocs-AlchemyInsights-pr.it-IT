---
title: Identificare l'attività delle regole di Posta in arrivo nei log di controllo
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976869"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificare l'attività delle regole di Posta in arrivo nei log di controllo

È possibile utilizzare la ricerca nei log di controllo nel Centro sicurezza & e conformità di Microsoft 365 per visualizzare gli eventi delle regole di posta in arrivo (creazione, modifica ed eliminazione di regole di Posta in arrivo).

1. Accedere al Centro [Microsoft 365 conformità](https://protection.office.com/).

2. Passare alla pagina **ricerca log** di  >  **controllo della** ricerca.

3. Selezionare l'intervallo di date nei **campi Data inizio** e Data **fine.**

4. In **Exchange cassette postali,** verificare che il **campo** Attività sia impostato su **New-InboxRule Creare/modificare/abilitare/disabilitare la regola di posta in arrivo.**

5. Fare clic su **Cerca**.

Nei risultati selezionare un record di controllo. Nel riquadro a comparsa dei dettagli fare clic **su Altre informazioni.** Le informazioni sulle impostazioni delle regole di Posta in arrivo vengono visualizzate nel **campo** Parametri.

Per ulteriori informazioni, vedere [Determining if a user created an Inbox rule](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
