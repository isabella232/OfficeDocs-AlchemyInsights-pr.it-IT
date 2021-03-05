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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464604"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Leggere i registri di controllo per gli eventi eliminati

Ecco come eseguire questa operazione:

1. Passare al Centro sicurezza e conformità di [Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Selezionare **Ricerca log** di  >  [**controllo**](https://go.microsoft.com/fwlink/?linkid=2103759).
    > [!NOTE]
    > Se viene visualizzato un avviso che indica che è necessario attivare la funzionalità, procedere e attivarla ora. Se la funzionalità non è attivata, i risultati della ricerca non saranno in grado di estrarre i dati dalle date precedenti.
1. Selezionare **Attività** e quindi individuare le **attività della cassetta postale di Exchange.** Selezionare le **opzioni Messaggi eliminati dalla cartella Posta** eliminata e Messaggi **spostati nella cartella** Posta eliminata. Al termine, fare clic all'esterno del riquadro per ridurre a icona il **riquadro** Attività.
1. Specificare l'intervallo di date e quindi nella **casella** Utenti selezionare il nome utente per l'utente che si desidera analizzare. È possibile selezionare più di un utente alla volta.
1. Selezionare **Cerca.** Le attività vengono visualizzate in **Risultati.**
1. Per visualizzare i dettagli, selezionare un'attività e quindi **selezionare Altre informazioni.** Ulteriori informazioni sull'elemento eliminato, ad esempio la riga dell'oggetto e la posizione dell'elemento al momento dell'eliminazione, vengono visualizzate nel campo **AffectedItems.**
    > [!NOTE]
    > Non è possibile ripristinare gli elementi eliminati utilizzando la funzionalità del log di controllo. Per ripristinare gli elementi eliminati, vedere [Recuperare gli elementi eliminati o la posta elettronica in Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)

Per ulteriori informazioni, vedere Eseguire una ricerca nel log di controllo di [Office 365 per risolvere i problemi relativi agli scenari comuni.](https://go.microsoft.com/fwlink/?linkid=2103944)
