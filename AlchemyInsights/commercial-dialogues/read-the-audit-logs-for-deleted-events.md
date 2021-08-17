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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896019"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Leggere i registri di controllo per gli eventi eliminati

Ecco come eseguire questa operazione:

1. Eseguire una delle operazioni seguenti:
   - Nell'Centro conformità Microsoft 365 <https://compliance.microsoft.com> in , passare a **Soluzioni** \> **Controllo**. In caso contrario, per passare direttamente alla **pagina Controllo,** utilizzare <https://compliance.microsoft.com/auditlogsearch> .
   - Nel portale di Microsoft 365 Defender <https://security.microsoft.com> all'indirizzo , passare a **Controlla**. In caso contrario, per passare direttamente alla **pagina Controllo,** utilizzare <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Se viene visualizzato un avviso che indica che è necessario attivare la funzionalità, procedere e attivarla ora. Se la funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.

2. Nella scheda **Ricerca** della pagina **Controllo** configurare le impostazioni seguenti:
   - **Intervallo di data e ora**: selezionare l'intervallo di data/ora nelle **caselle Inizio** **e** Fine.
   - **Attività**: immettere **Exchange attività della cassetta postale** e quindi selezionare i valori seguenti:
     - **Messaggi eliminati dalla cartella Posta eliminata**
     - **Messaggi spostati nella cartella Posta eliminata**

       Al termine, fare clic all'esterno del riquadro per ridurre a icona **il riquadro** Attività.

   - **Utenti**: accettare il valore predefinito vuoto per restituire i risultati per tutti gli utenti oppure immettere uno o più utenti.

3. Al termine, fare clic su **Cerca**. Le attività vengono visualizzate nella nuova **pagina Di ricerca di** controllo.

4. Selezionare un'attività nei risultati per aprire il riquadro a comparsa dei dettagli. Ulteriori informazioni sull'elemento eliminato, ad esempio la riga dell'oggetto e la posizione dell'elemento al momento dell'eliminazione, vengono visualizzate nel **campo AffectedItems.**

   > [!NOTE]
   > Non è possibile ripristinare gli elementi eliminati utilizzando la funzionalità del log di controllo. Per ripristinare gli elementi eliminati, vedere [Recover deleted email messages in Outlook sul web](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Per ulteriori informazioni, vedere [Search the audit log to investigate common support issues](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
