---
title: L'icona del calendario non viene visualizzata nel client di Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989595"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>L'icona del calendario non viene visualizzata nel client di Teams

La scheda Calendario in Teams richiede l'accesso a una cassetta postale di Exchange tramite i Servizi Web Exchange. La cassetta postale di Exchange può essere online o locale. Per gli utenti online che non vedono la scheda Calendario, accertarsi che [abbiano la licenza per una cassetta postale di Exchange Online e che la cassetta postale sia abilitata](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Se l'utente ha una cassetta postale valida in Exchange Online, ma non riesce ancora a visualizzare la scheda Calendario, può trattarsi di un problema di rete. Usare l'[Analizzatore connettività remota Microsoft](https://testconnectivity.microsoft.com/) ed eseguire i **Test di connettività dei servizi Web di Microsoft Exchange** per l'utente interessato.

Infine, controllare in [App di Teams - Criteri di installazione app](https://admin.teams.microsoft.com/policies/app-setup) che l'app Calendario non sia stata rimossa dal criterio applicato all'utente (probabilmente il criterio **Globale** predefinito a livello di organizzazione).

Se gli utenti sono ospitati in locale, è necessario verificare che l'integrità della configurazione ibrida. Usare la [Configurazione guidata ibrida](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) per la risoluzione dei problemi.

Si noti che [Teams richiede Exchange 2016 CU3 o versione successiva](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
