---
title: Criterio di condivisione del calendario 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373003"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Errore del criterio durante la condivisione di un calendario

1. Eseguire una delle operazioni seguenti, a seconda dei casi, per la situazione:
    - Connettersi a Exchange Online tramite Remote PowerShell. Per ulteriori informazioni, vedere [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Nel server locale, aprire Exchange Management Shell.
2. Determinare il criterio di condivisione assegnato all'utente. A tale scopo, eseguire il comando riportato di seguito e prendere nota del criterio restituito:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aggiornare il criterio di condivisione per l'utente. A tale scopo, attieniti alla seguente procedura:
    - Aprire l'interfaccia di amministrazione di Exchange.
    - Fare clic su **organizzazione**e quindi fare doppio clic sul criterio assegnato all'utente in **Condivisione singola**. Questo è il criterio che è stato restituito al passaggio 2.
    - Nella pagina regola di condivisione selezionare il livello di condivisione del calendario che si desidera consentire in **specificare le informazioni che si desidera condividere**. fare clic su **Salva**.

Per ulteriori informazioni, vedere: ["il criterio non consente di concedere autorizzazioni a questo livello a uno o più destinatari" errore quando l'utente tenta di condividere il calendario](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
