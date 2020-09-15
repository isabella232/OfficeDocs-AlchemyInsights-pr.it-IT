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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696517"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Registri di controllo per i messaggi di posta elettronica eliminati

A partire da gennaio 2019, Microsoft sta attivando la registrazione di controllo delle cassette postali per impostazione predefinita. In caso contrario, per esaminare eliminare gli eventi dei messaggi per un utente specifico, è necessario abilitare manualmente le azioni di eliminazione per il controllo. Se la registrazione di controllo delle cassette postali è già abilitata per l'organizzazione o per l'utente specifico, attenersi alla procedura seguente.

1. Accedere al [Centro sicurezza e conformità & Microsoft 365](https://protection.office.com/)

2. Fare clic su **ricerca e analisi** e selezionare **Ricerca log di controllo**.

3. Selezionare l'intervallo di date nei campi data di **inizio** e **Data di fine** . Specificare il nome utente per gli utenti che si desidera esaminare (l'utente che ha eliminato gli elementi). Nel campo **attività** selezionare **messaggi eliminati dalla cartella Posta eliminata** e **spostare i messaggi nella cartella Posta eliminata**.

4. Fare clic su **Cerca**.

Nei risultati, selezionare un record di controllo. Nel riquadro a comparsa dettagli, fare clic su **altre informazioni**. Ulteriori informazioni sull'elemento eliminato, ad esempio la riga dell'oggetto e la posizione dell'elemento quando è stata eliminata, vengono visualizzate nel campo **AffectedItems** . La proprietà **ClientInfoString** verrà visualizzata se l'eliminazione si è verificata in Outlook, Outlook sul Web (in precedenza noto come Outlook Web App) o qualsiasi altro dispositivo.

Per ulteriori informazioni, vedere [determinare chi ha configurato l'inoltro della posta elettronica per una cassetta postale](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Nota**: non è possibile recuperare gli elementi eliminati utilizzando la caratteristica log di controllo. Per recuperare i messaggi eliminati in Outlook sul Web, vedere [recuperare gli elementi eliminati in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
