---
title: 'Risoluzione dei problemi relativi alla segreteria telefonica '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: 36ba65c1ee67631a8b3c24c3407f46e3304541c5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330748"
---
# <a name="troubleshooting-voicemail"></a>Risoluzione dei problemi relativi alla segreteria telefonica

Verificare che la funzionalità Occupato su occupato sia intenzionale.

Se questa funzionalità non è necessaria per questo utente:

1. Passare a [Teams di amministrazione](https://admin.teams.microsoft.com/policies/calling).
1. Sul binario sinistro esplorare **Criteri di**  >  **chiamata vocale** Gestisci  >  **criteri** nel **criterio chiamante**.
1. Selezionare **Gestisci utenti**.
1. Cercare l'utente e modificare il criterio di chiamata in uno che ha occupato occupato è **disponibile quando in una chiamata a** **Off**.
1. Fare clic su **Applica**.

**Nota:** la replica delle modifiche ai criteri può richiedere fino a 24 ore.

Per ulteriori informazioni su questa funzionalità, vedere: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).
