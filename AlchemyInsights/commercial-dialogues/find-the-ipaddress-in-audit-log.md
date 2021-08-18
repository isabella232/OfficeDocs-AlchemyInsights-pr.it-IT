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
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902264"
---
# <a name="find-the-ip-address-in-audit-log"></a>Trovare l'indirizzo IP nel registro di controllo

L'indirizzo IP corrispondente a un'attività eseguita da un utente o da un amministratore viene visualizzato nei registri di controllo. Vengono registrate anche le informazioni sul client. Ecco come identificare l'indirizzo IP:

1. Eseguire una delle operazioni seguenti:
   - Nella finestra Centro conformità Microsoft 365 <https://compliance.microsoft.com> , passare a **Soluzioni** \> **Controllo**. In caso contrario, per passare direttamente alla **pagina Controllo,** utilizzare <https://compliance.microsoft.com/auditlogsearch> .
   - Nel portale Microsoft 365 Defender <https://security.microsoft.com> all'indirizzo , passare a **Controlla**. In caso contrario, per passare direttamente alla **pagina Controllo,** utilizzare <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora. Se questa funzionalità non è abilitata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.

2. Nella pagina **Controllo** verificare che la scheda **Ricerca** sia selezionata e quindi configurare le impostazioni seguenti:
   - **Intervallo di data e ora**: selezionare l'intervallo di data/ora nelle **caselle Inizio** **e** Fine.
   - **Attività:** se si è interessati a un'attività specifica, selezionarla nell'elenco. in caso contrario, verrà **restituito il valore** predefinito Mostra risultati per tutte le attività. Si noti che alcune attività potrebbero non essere disponibili per la selezione. Tuttavia, tali elementi di controllo verranno restituiti se **è selezionata l'opzione** Mostra risultati per tutte le attività.
   - **Utenti**: accettare il valore predefinito vuoto per restituire i risultati per tutti gli utenti oppure immettere uno o più utenti.

3. Al termine, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova **pagina Di ricerca di** controllo.

4. Nei risultati, fare clic **su Filtra risultati** e digitare **Set-Mailbox** nella casella filtro attività.

5. Selezionare un record di controllo nei risultati per aprire il **riquadro a comparsa** Dettagli.

Per ulteriori informazioni, vedere [Search the audit log to investigate common support issues](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
