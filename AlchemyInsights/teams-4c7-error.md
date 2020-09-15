---
title: Errore 4C7 Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700207"
---
# <a name="4c7-error-in-microsoft-teams"></a>errore 4C7 in Microsoft Teams

Questo errore si verifica perché Microsoft teams richiede l'autenticazione basata su form. Quando si distribuisce Active Directory Federation Services (AD FS), l'autenticazione basata su form non è abilitata per impostazione predefinita per la rete Intranet. Se l'autenticazione integrata di Windows ha esito negativo, viene richiesto di eseguire l'accesso utilizzando l'autenticazione basata su form.

Per risolvere il problema, abilitare l'autenticazione basata su form mediante lo snap-in di Microsoft Management Console (MMC) di ADFS nel computer in cui è presente la copia locale di Active Directory. A tal fine, attenersi alla seguente procedura: 

1. Nel riquadro di spostamento, passare a **criteri di autenticazione**.
2. In **azioni** nel riquadro dei dettagli, selezionare **Modifica autenticazione primaria globale**.
3. Nella scheda **Intranet** selezionare **autenticazione Forms**.
4. Fare clic su **OK** (o su **applica**).