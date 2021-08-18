---
title: Ottenere i log di controllo
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/16/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10964"
- "3100005"
ms.openlocfilehash: ac2e5eafbb92b234697c22f73cd565af9d7c3508
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329498"
---
# <a name="retrieve-the-audit-logs"></a>Ottenere i log di controllo

Quando si apre per la prima volta un log di controllo, questo è vuoto. È necessario effettuare una ricerca per analizzare il contenuto. Ecco come eseguire una ricerca generale per tutte le attività:

1. Eseguire uno dei seguenti passaggi:
   - Nel Centro conformità Microsoft 365 in <https://compliance.microsoft.com>, passare a **Soluzioni** \> **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://compliance.microsoft.com/auditlogsearch>.
   - Nel portale di Microsoft 365 Defender in <https://security.microsoft.com>, passare ad **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://sip.security.microsoft.com/auditlogsearch>.

2. Alla pagina **Audit**, verificare che la scheda **Cerca** sia selezionata e configurare le seguenti impostazioni:
   - **Intervallo di data e ora**: selezionare l'intervallo di data/ora nelle caselle **Inizio** e **Fine**.
   - **Attività**: verificare che **Mostra risultati per tutte le attività** sia selezionato.
   - **Utenti**: accettare il valore predefinito vuoto per restituire i risultati di tutti gli utenti, oppure immettere uno o più utenti.

3. Una volta terminato, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova pagina **Ricerca audit**.

4. Nei risultati, fare clic su **Filtra risultati** e digitare **Set-Mailbox** nella casella filtro attività.

5. Selezionare un record di audit nei risultati. Nel menu a comparsa **Dettagli**, fare clic su **Altre informazioni** per visualizzare altre informazioni quali Client, Utente che ha eseguito l'azione, ecc.
