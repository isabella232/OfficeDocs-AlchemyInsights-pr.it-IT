---
title: Analizzare tutte le attività degli utenti
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332347"
---
# <a name="investigate-all-the-users-activities"></a>Analizzare tutte le attività degli utenti

Ecco come eseguire questa operazione:

1. Eseguire una delle operazioni seguenti:
   - Nel Centro conformità Microsoft 365 in <https://compliance.microsoft.com>, passare a **Soluzioni** \> **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://compliance.microsoft.com/auditlogsearch>.
   - Nel portale di Microsoft 365 Defender in <https://security.microsoft.com>, passare ad **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://security.microsoft.com/auditlogsearch>.

    **Nota:** se viene visualizzato un avviso che indica che è necessario attivare la funzionalità, procedere e attivarla ora. Se la funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.

2. Nella scheda **Ricerca** della pagina **Controllo** configurare le impostazioni seguenti:
   - **Intervallo di data e ora**: selezionare l'intervallo di data/ora nelle caselle **Inizio** e **Fine**.
   - **Attività:** se si è interessati a un'attività specifica, selezionarla nell'elenco. in caso contrario, il valore predefinito **Mostra risultati per tutte le attività** restituisce tutte le attività.
   - **Utenti**: accettare il valore predefinito vuoto per restituire i risultati di tutti gli utenti, oppure immettere uno o più utenti.

3. Una volta terminato, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova pagina **Ricerca audit**. Verranno visualizzati **l'indirizzo IP,** **l'utente** e il **nome dell'attività.**

4. Per scaricare i risultati, selezionare **Esporta** \> **Scarica tutti i risultati**.

5. Selezionare un'attività nei risultati per aprire il riquadro a comparsa dei dettagli.

Per ulteriori informazioni, vedere [Search the audit log to investigate common support issues](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
