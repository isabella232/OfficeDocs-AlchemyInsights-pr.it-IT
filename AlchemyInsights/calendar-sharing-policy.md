---
title: Criterio di condivisione del calendario 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684234"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Errore del criterio durante la condivisione di un calendario

1. Eseguire una delle operazioni seguenti, a seconda dei casi, per la situazione:
    - Connettersi a Exchange Online tramite Remote PowerShell. Per ulteriori informazioni, vedere [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Nel server locale, aprire Exchange Management Shell.
2. Determinare il criterio di condivisione assegnato all'utente. A tale scopo, eseguire il comando riportato di seguito e prendere nota del criterio restituito:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aggiornare il criterio di condivisione per l'utente. A tal fine, attenersi alla seguente procedura:
    - Aprire l'interfaccia di amministrazione di Exchange.
    - Fare clic su **organizzazione**e quindi fare doppio clic sul criterio assegnato all'utente in **Condivisione singola**. Questo è il criterio che è stato restituito al passaggio 2.
    - Nella pagina regola di condivisione selezionare il livello di condivisione del calendario che si desidera consentire in **specificare le informazioni che si desidera condividere**. fare clic su **Salva**.

Per ulteriori informazioni, vedere: ["il criterio non consente di concedere autorizzazioni a questo livello a uno o più destinatari" errore quando l'utente tenta di condividere il calendario](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
