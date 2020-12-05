---
title: L'icona del calendario non viene visualizzata nel client Microsoft Teams
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
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576519"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>L'icona del calendario non viene visualizzata nel client Microsoft Teams

La scheda **Calendario** in teams richiede l'accesso a una cassetta postale di Exchange tramite i servizi Web di Exchange. La cassetta postale di Exchange può essere online o locale. Per gli utenti online che non vedono la scheda **Calendario** , accertarsi che [siano concessi in licenza per una cassetta postale di Exchange Online e che la cassetta postale sia abilitata](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Se gli utenti sono ospitati in locale, è necessario verificare che la configurazione ibrida sia integra. Usare la [Configurazione ibrida guidata](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) per la risoluzione dei problemi. Si noti che [Teams richiede Exchange 2016 CU3 o versione successiva](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Per ulteriori informazioni e procedure per la risoluzione dei problemi, vedere risolvere i problemi relativi all' [interazione di Microsoft teams e Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).
