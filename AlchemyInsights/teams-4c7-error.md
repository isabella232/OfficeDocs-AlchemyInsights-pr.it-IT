---
title: Teams errore 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049312"
---
# <a name="4c7-error-in-microsoft-teams"></a>Errore 4c7 in Microsoft Teams

Questo errore si verifica perché Microsoft Teams richiede l'autenticazione Forms. Quando si distribuisce Active Directory Federation Services (ADFS), l'autenticazione Forms non è abilitata per la rete Intranet per impostazione predefinita. Se Windows'autenticazione integrata ha esito negativo, viene richiesto di accedere utilizzando l'autenticazione Forms.

Per risolvere questo problema, abilitare l'autenticazione Forms utilizzando lo snap-in AD FS Microsoft Management Console (MMC) nel computer che dispone della copia locale di Active Directory. A tale scopo, eseguire la procedura seguente: 

1. Nel riquadro di spostamento passare a **Criteri di autenticazione.**
2. In **Azioni** nel riquadro dei dettagli selezionare **Modifica autenticazione principale globale**.
3. Nella scheda **Intranet** selezionare **Autenticazione Forms**.
4. Selezionare **OK** (o **Applica**).