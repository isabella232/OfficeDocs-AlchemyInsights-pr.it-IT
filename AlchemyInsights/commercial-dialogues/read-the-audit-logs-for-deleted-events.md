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
ms.openlocfilehash: 8d656d5660b7c6e6d32d32a06c3dbf49c45e4ca04c4422128f1c4ea62413afa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967337"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Leggere i registri di controllo per gli eventi eliminati

Ecco come eseguire questa operazione:

1. Passare al Centro [Office 365 sicurezza & conformità](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Selezionare **Ricerca**  >  [**log di controllo ricerca**](https://go.microsoft.com/fwlink/?linkid=2103759).
    > [!NOTE]
    > Se viene visualizzato un avviso che indica che è necessario attivare la funzionalità, procedere e attivarla ora. Se la funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.
1. Selezionare **Attività** e quindi individuare le attività **Exchange cassetta postale.** Selezionare le **opzioni Messaggi eliminati dalla cartella Posta** eliminata e Messaggi **spostati nella cartella Posta** eliminata. Al termine, fare clic all'esterno del riquadro per ridurre a icona **il riquadro** Attività.
1. Specificare l'intervallo di date e quindi nella **casella Utenti** selezionare il nome utente dell'utente che si desidera analizzare. È possibile selezionare più di un utente alla volta.
1. Selezionare **Cerca**. Le attività vengono visualizzate in **Risultati**.
1. Per visualizzare i dettagli, selezionare un'attività e quindi **selezionare Altre informazioni.** Ulteriori informazioni sull'elemento eliminato, ad esempio la riga dell'oggetto e la posizione dell'elemento al momento dell'eliminazione, vengono visualizzate nel **campo AffectedItems.**
    > [!NOTE]
    > Non è possibile ripristinare gli elementi eliminati utilizzando la funzionalità del log di controllo. Per ripristinare gli elementi eliminati, vedere [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).

Per ulteriori informazioni, vedere [Search the Office 365 audit log to troubleshoot common scenarios.](https://go.microsoft.com/fwlink/?linkid=2103944)
