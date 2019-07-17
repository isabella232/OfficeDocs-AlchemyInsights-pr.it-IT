---
title: Dynamics 365-il dashboard errato viene visualizzato nell'interfaccia unificata di Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747989"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Il dashboard errato viene visualizzato nell'interfaccia unificata di Dynamics 365

Vi sono diversi motivi per cui è possibile che venga visualizzato un dashboard diverso da quello previsto:

## <a name="the-user-has-set-a-user-default-dashboard"></a>L'utente ha impostato un dashboard predefinito dell'utente 

In genere è possibile identificare un dashboard predefinito utente è impostato se il pulsante **Imposta come predefinito** non viene visualizzato nella barra dei comandi del dashboard. Il dashboard predefinito dell'utente sostituirà tutti gli altri dashboard predefiniti, anche se il dashboard predefinito dell'utente non è incluso nell'app corrente.

Per annullare il dashboard predefinito, utilizzare la soluzione seguente.

1. Creare un nuovo dashboard personale.

2. Impostare il nuovo dashboard come predefinito dell'utente.

3. Eliminare il dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Il dashboard è impostato nella mappa del sito.

È possibile che sia stato impostato un dashboard predefinito dell'organizzazione selezionando un dashboard e scegliendo ' imposta come predefinito ' in ' Personalizza il sistema '. Tuttavia, il dashboard definito nella Sitemap designer avrà la precedenza su questo dashboard, se l'utente può accedervi.

Per consentire agli utenti di visualizzare il dashboard impostato come predefinito dell'organizzazione, è possibile eseguire le operazioni seguenti:

* Impostare il dashboard nella Sitemap

* Rimuovere l'accesso al dashboard definito Sitemap per tali utenti
