---
title: 618 Criteri di condivisione del calendario
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091607"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Errore dei criteri durante la condivisione di un calendario

1. Eseguire una delle operazioni seguenti, in base alle proprie esigenze:
    - Connessione per Exchange Online tramite Remote PowerShell. Per ulteriori informazioni, [vedere Connessione to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Nel server locale, aprire la Exchange Management Shell.
2. Determinare il criterio di condivisione assegnato all'utente. A tale scopo, eseguire il comando seguente e prendere nota del criterio restituito:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Aggiornare i criteri di condivisione per l'utente. A tale scopo, eseguire la procedura seguente:
    - Aprire l'interfaccia di amministrazione di Exchange.
    - Fare **clic su** Organizzazione e quindi fare doppio clic sul criterio assegnato all'utente in Condivisione **individuale.** Si tratta del criterio restituito nel passaggio 2.
    - Nella pagina Regola di condivisione selezionare il livello di condivisione del calendario che si desidera consentire in Specificare le **informazioni che si desidera condividere.** fare **clic su Salva**.

Per ulteriori informazioni, vedere: Errore "I criteri non consentono la concessione delle autorizzazioni a questo livello a uno o più destinatari" quando l'utente tenta di [condividere il calendario.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
