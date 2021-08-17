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
ms.openlocfilehash: d05c8f02efc3bb92865880ea4a2338abaf7d70254f0b4bbfb566423e62b391dd
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898800"
---
# <a name="investigate-all-the-users-activities"></a>Analizzare tutte le attività degli utenti

Ecco come eseguire questa operazione:

1. Eseguire una delle operazioni seguenti:
   - Nella finestra Centro conformità Microsoft 365 <https://compliance.microsoft.com> , passare a **Soluzioni** \> **Controllo**. In caso contrario, per passare direttamente alla **pagina Controllo,** utilizzare <https://compliance.microsoft.com/auditlogsearch> .
   - Nel portale Microsoft 365 Defender <https://security.microsoft.com> all'indirizzo , passare a **Controlla**. In caso contrario, per passare direttamente alla **pagina Controllo,** utilizzare <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Se viene visualizzato un avviso che indica che è necessario attivare la funzionalità, procedere e attivarla ora. Se la funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.

2. Nella scheda **Ricerca** della pagina **Controllo** configurare le impostazioni seguenti:
   - **Intervallo di data e ora**: selezionare l'intervallo di data/ora nelle **caselle Inizio** **e** Fine.
   - **Attività:** se si è interessati a un'attività specifica, selezionarla nell'elenco. in caso contrario, il valore predefinito **Mostra risultati per tutte le attività** restituisce tutte le attività.
   - **Utenti**: accettare il valore predefinito vuoto per restituire i risultati per tutti gli utenti oppure immettere uno o più utenti.

3. Al termine, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova **pagina Di ricerca di** controllo. Verranno visualizzati **l'indirizzo IP,** **l'utente** e il **nome dell'attività.**

4. Per scaricare i risultati, selezionare **Esporta** \> **Scarica tutti i risultati**.

5. Selezionare un'attività nei risultati per aprire il riquadro a comparsa dei dettagli.

Per ulteriori informazioni, vedere [Search the audit log to investigate common support issues](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
