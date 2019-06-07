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
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752064"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificare l'indirizzo IP e il client nei registri di controllo

L'indirizzo IP corrispondente a un'attività di un utente o di un amministratore viene visualizzato nei registri di controllo. Vengono inoltre registrate le informazioni sul client. Di seguito vengono illustrati i passaggi per identificare tali informazioni

1. Accedere al [Centro sicurezza & conformità di Office 365](https://protection.office.com/)

2. Fare clic su **ricerca e analisi** e selezionare **Ricerca log di controllo**.

   Se si è interessati a un'attività specifica, selezionarla dall'elenco **attività** . In caso contrario, verranno restituite tutte le attività per l'utente selezionato (impostazione predefinita).

   **Nota**: alcune attività potrebbero non essere disponibili nel menu **attività** ; Tuttavia, tali elementi di controllo verranno restituiti se è selezionata l'opzione **Mostra risultati per tutte le attività** (impostazione predefinita).

3. Specificare il nome utente nel campo **utenti** , selezionare l'intervallo di date appropriato per l'attività, quindi fare clic su **Cerca**.

Nei risultati, è possibile visualizzare l'indirizzo IP per tale attività nel riquadro dei risultati. Selezionare il record di controllo per visualizzare informazioni dettagliate nel riquadro a comparsa dei **Dettagli** , ad esempio client, utente che ha eseguito un'azione e così via.

Per ulteriori informazioni, vedere [trovare l'indirizzo IP del computer utilizzato per accedere a un account compromesso](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
