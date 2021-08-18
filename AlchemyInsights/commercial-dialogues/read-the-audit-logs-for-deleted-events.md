---
title: Leggere i registri di controllo per gli eventi eliminati
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324737"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Leggere i registri di controllo per gli eventi eliminati

Ecco come eseguire questa operazione:

1. Eseguire una delle operazioni seguenti:
   - Nel Centro conformità Microsoft 365 in <https://compliance.microsoft.com>, passare a **Soluzioni** \> **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://compliance.microsoft.com/auditlogsearch>.
   - Nel portale di Microsoft 365 Defender in <https://security.microsoft.com>, passare ad **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://security.microsoft.com/auditlogsearch>.

    **Nota:** se viene visualizzato un avviso che indica che è necessario attivare la funzionalità, procedere e attivarla ora. Se la funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.

2. Nella scheda **Ricerca** della pagina **Controllo** configurare le impostazioni seguenti:
   - **Intervallo di data e ora**: selezionare l'intervallo di data/ora nelle caselle **Inizio** e **Fine**.
   - **Attività**: immettere **Exchange attività della cassetta postale** e quindi selezionare i valori seguenti:
     - **Messaggi eliminati dalla cartella Posta eliminata**
     - **Messaggi spostati nella cartella Posta eliminata**

       Al termine, fare clic all'esterno del riquadro per ridurre a icona **il riquadro** Attività.

   - **Utenti**: accettare il valore predefinito vuoto per restituire i risultati di tutti gli utenti, oppure immettere uno o più utenti.

3. Una volta terminato, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova pagina **Ricerca audit**.

4. Selezionare un'attività nei risultati per aprire il riquadro a comparsa dei dettagli. Ulteriori informazioni sull'elemento eliminato, ad esempio la riga dell'oggetto e la posizione dell'elemento al momento dell'eliminazione, vengono visualizzate nel **campo AffectedItems.**

   **Nota:** non è possibile ripristinare gli elementi eliminati utilizzando la funzionalità del log di controllo. Per ripristinare gli elementi eliminati, vedere [Recover deleted email messages in Outlook sul web](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Per ulteriori informazioni, vedere [Search the audit log to investigate common support issues](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
