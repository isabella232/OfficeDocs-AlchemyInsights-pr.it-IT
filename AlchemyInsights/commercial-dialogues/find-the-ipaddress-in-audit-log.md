---
title: Trovare l'indirizzo IP nel registro di controllo
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
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303581"
---
# <a name="find-the-ip-address-in-audit-log"></a>Trovare l'indirizzo IP nel registro di controllo

L'indirizzo IP corrispondente a un'attività eseguita da un utente o da un amministratore viene visualizzato nei registri di controllo. Vengono registrate anche le informazioni sul client. Ecco come identificare l'indirizzo IP:

1. Eseguire una delle operazioni seguenti:
   - Nel Centro conformità Microsoft 365 in <https://compliance.microsoft.com>, passare a **Soluzioni** \> **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://compliance.microsoft.com/auditlogsearch>.
   - Nel portale di Microsoft 365 Defender in <https://security.microsoft.com>, passare ad **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://security.microsoft.com/auditlogsearch>.

    **Nota:** se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora. Se questa funzionalità non è abilitata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.

2. Alla pagina **Audit**, verificare che la scheda **Cerca** sia selezionata e configurare le seguenti impostazioni:
   - **Intervallo di data e ora**: selezionare l'intervallo di data/ora nelle caselle **Inizio** e **Fine**.
   - **Attività:** se si è interessati a un'attività specifica, selezionarla nell'elenco. in caso contrario, verrà **restituito il valore** predefinito Mostra risultati per tutte le attività. Si noti che alcune attività potrebbero non essere disponibili per la selezione. Tuttavia, tali elementi di controllo verranno restituiti se **è selezionata l'opzione** Mostra risultati per tutte le attività.
   - **Utenti**: accettare il valore predefinito vuoto per restituire i risultati di tutti gli utenti, oppure immettere uno o più utenti.

3. Una volta terminato, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova pagina **Ricerca audit**.

4. Nei risultati, fare clic su **Filtra risultati** e digitare **Set-Mailbox** nella casella filtro attività.

5. Selezionare un record di controllo nei risultati per aprire il **riquadro a comparsa** Dettagli.

Per ulteriori informazioni, vedere [Search the audit log to investigate common support issues](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
