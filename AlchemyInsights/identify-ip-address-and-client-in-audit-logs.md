---
title: Identificare l'indirizzo IP e il client nei log di controllo
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313023"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identificare l'indirizzo IP e il client nei log di controllo

L'indirizzo IP corrispondente a un'attività di un Microsoft 365 utente o amministratore viene visualizzato nei registri di controllo. Vengono registrate anche le informazioni sul client. Ecco i passaggi per identificare tali informazioni

1. Accedere al Centro [Microsoft 365 conformità](https://protection.office.com/).

2. Passare alla pagina **ricerca log** di  >  **controllo della** ricerca.

   Se si è interessati a un'attività specifica, selezionarla **nell'elenco** Attività. In caso contrario, verranno restituite tutte le attività per l'utente selezionato (impostazione predefinita).

   **Nota:** alcune attività potrebbero non essere disponibili nel menu **Attività.** Tuttavia, tali elementi di controllo verranno restituiti se è selezionata **l'opzione Mostra risultati per tutte** le attività (impostazione predefinita).

3. Specificare il nome utente nel **campo Utenti,** selezionare l'intervallo di date appropriato per l'attività e quindi fare clic su **Cerca.**

Nei risultati è possibile visualizzare l'indirizzo IP dell'attività nel riquadro dei risultati. Selezionare il record di controllo per  visualizzare informazioni dettagliate nel riquadro a comparsa Dettagli, ad esempio Client, Utente che ha eseguito l'azione e così via.

Per ulteriori informazioni, vedere [Individuazione dell'indirizzo IP del computer utilizzato per accedere a un account compromesso.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
