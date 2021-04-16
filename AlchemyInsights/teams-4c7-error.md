---
title: Errore di Teams 4c7
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
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786673"
---
# <a name="4c7-error-in-microsoft-teams"></a>Errore 4c7 in Microsoft Teams

Questo errore si verifica perché Microsoft Teams richiede l'autenticazione Forms. Quando si distribuisce Active Directory Federation Services (ADFS), l'autenticazione Forms non è abilitata per la rete Intranet per impostazione predefinita. Se l'autenticazione integrata di Windows non riesce, viene richiesto di accedere utilizzando l'autenticazione Forms.

Per risolvere questo problema, abilitare l'autenticazione Forms utilizzando lo snap-in AD FS Microsoft Management Console (MMC) nel computer che dispone della copia locale di Active Directory. A tal fine, attenersi alla seguente procedura: 

1. Nel riquadro di spostamento passare a **Criteri di autenticazione.**
2. In **Azioni** nel riquadro dei dettagli selezionare **Modifica autenticazione principale globale**.
3. Nella scheda **Intranet** selezionare **Autenticazione Forms**.
4. Selezionare **OK** (o **Applica**).