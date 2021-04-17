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
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819957"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>L'icona del calendario non viene visualizzata nel client di Teams

La scheda Calendario in Teams richiede l'accesso a una cassetta postale di Exchange tramite i Servizi Web Exchange. La cassetta postale di Exchange può essere online o locale. Per gli utenti online che non vedono la scheda Calendario, accertarsi che [abbiano la licenza per una cassetta postale di Exchange Online e che la cassetta postale sia abilitata](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Se l'utente ha una cassetta postale valida in Exchange Online, ma non riesce ancora a visualizzare la scheda Calendario, può trattarsi di un problema di rete. Usare l'[Analizzatore connettività remota Microsoft](https://testconnectivity.microsoft.com/) ed eseguire i **Test di connettività dei servizi Web di Microsoft Exchange** per l'utente interessato.

Infine, controllare in [App di Teams - Criteri di installazione app](https://admin.teams.microsoft.com/policies/app-setup) che l'app Calendario non sia stata rimossa dal criterio applicato all'utente (probabilmente il criterio **Globale** predefinito a livello di organizzazione).

Se gli utenti sono ospitati in locale, è necessario verificare che l'integrità della configurazione ibrida. Usare la [Configurazione ibrida guidata](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) per la risoluzione dei problemi.

Si noti che [Teams richiede Exchange 2016 CU3 o versione successiva](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
