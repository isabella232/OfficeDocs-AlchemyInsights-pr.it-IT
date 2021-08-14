---
title: Identificare gli eventi di eliminazione dei messaggi nei registri di controllo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f68b623abd0efa990df71e5bf1ea1c9e7367ed691b1752f68c971e973922a63d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868422"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Log di controllo per i messaggi di posta elettronica eliminati

A partire da gennaio 2019, Microsoft attiva la registrazione di controllo delle cassette postali per impostazione predefinita. In caso contrario, per esaminare gli eventi di eliminazione dei messaggi per un utente specifico, è necessario abilitare manualmente le azioni di eliminazione per il controllo. Se la registrazione di controllo delle cassette postali è già abilitata per l'organizzazione o per l'utente specifico, eseguire la procedura seguente.

1. Accedere al Centro [Microsoft 365 conformità](https://protection.office.com/)

2. Fare **clic su Ricerca e analisi** e selezionare Ricerca log di **controllo**.

3. Selezionare l'intervallo di date nei **campi Data inizio** e Data **fine.** Specificare il nome utente per l'utente che si desidera analizzare (l'utente che ha eliminato gli elementi). Nel campo **Attività** selezionare **Messaggi eliminati dalla cartella Posta eliminata** e Messaggi **spostati nella cartella Posta eliminata**.

4. Fare clic su **Cerca**.

Nei risultati selezionare un record di controllo. Nel riquadro a comparsa dei dettagli fare clic **su Altre informazioni.** Ulteriori informazioni sull'elemento eliminato, ad esempio la riga dell'oggetto e la posizione dell'elemento al momento dell'eliminazione, vengono visualizzate nel **campo AffectedItems.** La **proprietà ClientInfoString** mostrerà se l'eliminazione si è verificata in Outlook, Outlook sul web (in precedenza noto come Outlook Web App) o in qualsiasi altro dispositivo.

Per ulteriori informazioni, vedere [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Nota:** non è possibile recuperare gli elementi eliminati utilizzando la funzionalità del log di controllo. Per recuperare i messaggi eliminati in Outlook sul web, vedere [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
