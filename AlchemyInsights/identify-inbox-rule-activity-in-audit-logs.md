---
title: Identificare la regola di posta in arrivo nei registri di controllo
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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779055"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificare la regola di posta in arrivo nei registri di controllo

È possibile utilizzare la ricerca del registro di controllo nel centro sicurezza & conformità di Microsoft 365 per visualizzare gli eventi delle regole di posta in arrivo (creazione, modifica ed eliminazione delle regole di posta in arrivo).

1. Accedere al [Centro sicurezza & conformità di Microsoft 365](https://protection.office.com/).

2. Passare alla pagina di ricerca del registro di controllo della **ricerca**  >  **Audit log search** .

3. Selezionare l'intervallo di date nei campi data di **inizio** e **Data di fine** .

4. In **attività Cassetta postale di Exchange**, verificare che il campo **attività** sia impostato su **nuovo-InboxRule creare/modificare/abilitare/disabilitare la regola di posta in arrivo**.

5. Fare clic su **Cerca**.

Nei risultati, selezionare un record di controllo. Nel riquadro a comparsa dettagli, fare clic su **altre informazioni**. Le informazioni sulle impostazioni delle regole di posta in arrivo vengono visualizzate nel campo **parametri** .

Per ulteriori informazioni, vedere [determinare se un utente ha creato una regola di posta in arrivo](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
