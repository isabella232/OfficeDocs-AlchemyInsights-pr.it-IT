---
title: L'icona calendario non viene visualizzata Microsoft Teams client
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120008"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>L'icona calendario non viene visualizzata Microsoft Teams client

La **scheda** Calendario in Teams richiede l'accesso a Exchange cassetta postale tramite Exchange Web Services. La Exchange può essere online o locale. Per gli utenti online che non visualizzano **la** scheda Calendario, assicurarsi che siano concessi in licenza per una cassetta postale Exchange Online e che la cassetta postale [sia abilitata.](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes) Se gli utenti sono ospitati in locale, è necessario verificare che la configurazione ibrida sia integra. Usare la [Configurazione ibrida guidata](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) per la risoluzione dei problemi. Si noti che [Teams richiede Exchange 2016 CU3 o versione successiva](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Per ulteriori informazioni e procedure per la risoluzione dei problemi, [vedere Risoluzione dei Microsoft Teams e Exchange Server di interazione.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
