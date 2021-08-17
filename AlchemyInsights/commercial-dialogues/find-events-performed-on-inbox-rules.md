---
title: Trovare gli eventi eseguiti sulle regole di Posta in arrivo
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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313503"
---
# <a name="find-events-performed-on-inbox-rules"></a>Trovare gli eventi eseguiti sulle regole di Posta in arrivo

Quando le regole della posta in arrivo vengono create, modificate o eliminate, gli eventi vengono registrati nel registro di controllo. Ecco come esaminarli:

1. Eseguire una delle operazioni seguenti:
   - Nel Centro conformità Microsoft 365 in <https://compliance.microsoft.com>, passare a **Soluzioni** \> **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://compliance.microsoft.com/auditlogsearch>.
   - Nel portale di Microsoft 365 Defender in <https://security.microsoft.com>, passare ad **Audit**. In alternativa, per passare direttamente alla pagina **Audit**, usare <https://security.microsoft.com/auditlogsearch>.

    **Nota:** se viene visualizzato un avviso che indica che è necessario attivare il controllo, procedere e attivarlo ora. Se questa funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.
1. Selezionare il campo Attività e individuare Exchange delle cassette postali, quindi selezionare New-InboxRule Crea regola posta in arrivo da Outlook Web App. Al termine, fare clic all'esterno del riquadro per ridurre a icona il riquadro Attività.
1. Specificare l'intervallo di date e quindi nel campo Utenti selezionare il nome utente per l'utente che si desidera analizzare. È possibile selezionare più di un utente alla volta.
1. Selezionare Cerca. Le attività vengono visualizzate in Risultati.
1. Per visualizzare i dettagli, selezionare un'attività e quindi selezionare Altre informazioni. Nella sezione Parametri è possibile visualizzare il nome della regola, il set di condizioni e le azioni che verranno eseguite dalla regola.

2. Nella scheda **Ricerca** della pagina **Controllo** configurare le impostazioni seguenti:
   - **Intervallo di data e ora**: selezionare l'intervallo di data/ora nelle caselle **Inizio** e **Fine**.
   - **Attività:** selezionare **New-InboxRule Crea regola di posta in arrivo da Outlook Web App**

3. Una volta terminato, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova pagina **Ricerca audit**.

4. Selezionare un'attività nei risultati per aprire il riquadro a comparsa dei dettagli. Nella sezione **Parametri** è possibile visualizzare il nome della regola, il set di condizioni e le azioni che verranno eseguite dalla regola.

Per ulteriori informazioni, vedere [Search the audit log to investigate common support issues](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
