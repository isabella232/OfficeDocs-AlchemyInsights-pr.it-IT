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
ms.openlocfilehash: e639d74cd8dbbb03ffb5b253451c99c8fe639f024a46e173845a0f4d322e43ca
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972387"
---
# <a name="troubleshooting-voicemail"></a>Risoluzione dei problemi relativi alla segreteria telefonica

Verificare che la funzionalità Occupato su occupato sia intenzionale.

Se questa funzionalità non è necessaria per questo utente:

1. Passare a [Teams di amministrazione](https://admin.teams.microsoft.com/policies/calling).
1. Sul binario sinistro esplorare **Criteri di**  >  **chiamata vocale** Gestisci  >  **criteri** nel **criterio chiamante**.
1. Selezionare **Gestisci utenti**.
1. Cercare l'utente e modificare il criterio di chiamata in uno che ha occupato occupato è **disponibile quando in una chiamata a** **Off**.
1. Fare clic su **Applica**.
> [!NOTE]
> La replica delle modifiche ai criteri può richiedere fino a 24 ore.

Per ulteriori informazioni su questa funzionalità, vedere: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).
