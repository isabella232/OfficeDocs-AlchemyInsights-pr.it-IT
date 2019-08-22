---
title: Identificare l'indirizzo IP e il client nei registri di controllo
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539033"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificare l'indirizzo IP e il client nei registri di controllo

L'indirizzo IP che corrisponde a un'attività di un utente o di un amministratore di Office 365 è visualizzato nei registri di controllo. Vengono inoltre registrate le informazioni sul client. Di seguito vengono illustrati i passaggi per identificare tali informazioni

1. Accedere al [Centro sicurezza & conformità di Office 365](https://protection.office.com/).

2. Passare alla pagina di**ricerca del registro di controllo** della **ricerca** > .

   Se si è interessati a un'attività specifica, selezionarla dall'elenco **attività** . In caso contrario, verranno restituite tutte le attività per l'utente selezionato (impostazione predefinita).

   **Nota**: alcune attività potrebbero non essere disponibili nel menu **attività** ; Tuttavia, tali elementi di controllo verranno restituiti se è selezionata l'opzione **Mostra risultati per tutte le attività** (impostazione predefinita).

3. Specificare il nome utente nel campo **utenti** , selezionare l'intervallo di date appropriato per l'attività, quindi fare clic su **Cerca**.

Nei risultati, è possibile visualizzare l'indirizzo IP per tale attività nel riquadro dei risultati. Selezionare il record di controllo per visualizzare informazioni dettagliate nel riquadro a comparsa dei **Dettagli** , ad esempio client, utente che ha eseguito un'azione e così via.

Per ulteriori informazioni, vedere [trovare l'indirizzo IP del computer utilizzato per accedere a un account compromesso](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
