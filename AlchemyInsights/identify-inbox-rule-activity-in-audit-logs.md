---
title: Identificare la regola di posta in arrivo nei registri di controllo
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909342"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identificare la regola di posta in arrivo nei registri di controllo

È possibile utilizzare la ricerca del registro di controllo nel centro sicurezza & Compliance per visualizzare gli eventi delle regole di posta in arrivo (creazione, modifica ed eliminazione delle regole di posta in arrivo).

1. Accedere al [centro conformità _AMP_ sicurezza di Office 365](https://protection.office.com/)

2. Fare clic su **ricerca e analisi** e selezionare **Ricerca log di controllo**.

3. Selezionare l'intervallo di date nei campi data di **inizio** e **Data di fine** .

4. In **attività Cassetta postale di Exchange**, verificare che il campo **attività** sia impostato su **nuovo-InboxRule creare/modificare/abilitare/disabilitare la regola di posta in arrivo**.

5. Fare clic su **Cerca**.

Nei risultati, selezionare un record di controllo. Nel riquadro a comparsa dettagli, fare clic su **altre informazioni**. Le informazioni sulle impostazioni delle regole di posta in arrivo vengono visualizzate nel campo **parametri** .

Per ulteriori informazioni, vedere [determinare se un utente ha creato una regola di posta in arrivo](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
