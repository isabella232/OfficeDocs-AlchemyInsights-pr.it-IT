---
title: Outlook desktop richiamare o sostituire un messaggio di posta elettronica
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663994"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Richiamare o sostituire un messaggio di posta elettronica di Outlook

- Come amministratore, è possibile **richiamare i messaggi per conto di utenti che utilizzano PowerShell**. Non è possibile richiamare messaggi dall'interfaccia di amministrazione.
- È possibile **richiamare solo i messaggi inviati alle persone all'interno dell'organizzazione**. Se il messaggio è stato inviato a un indirizzo Gmail, ad esempio, non è possibile richiamarlo.
- È possibile **richiamare solo i messaggi inviati da Outlook 2016 sul PC**. Se un utente invia un messaggio utilizzando Outlook per Mac o Outlook sul Web, non è possibile richiamarlo.

Per richiamare o sostituire un messaggio di posta elettronica:

1. Nel riquadro delle cartelle nella parte sinistra della finestra di Outlook selezionare la cartella posta inviata.
1. Fare doppio clic sul messaggio che si desidera richiamare per aprirlo.
1. Selezionare la scheda **messaggio** e quindi fare clic su **azioni**  >  **richiamare questo messaggio**.
1. Selezionare **Elimina copie non lette del messaggio** o **Elimina copie non lette e Sostituisci con un nuovo messaggio**e quindi fare clic su **OK**.
1. Se si sta inviando un messaggio di sostituzione, comporre il messaggio, quindi selezionare **Invia**.
1. L'esito positivo o negativo di un messaggio di richiamo dipende dalle impostazioni del destinatario in Outlook. Per la procedura da eseguire per la verifica del richiamo, vedere [questo articolo](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Cercare ed eliminare messaggi di posta elettronica nell'organizzazione

- Se non si è un amministratore globale, è necessario aggiungere l'account al ruolo eDiscovery Manager o alla funzione di gestione della ricerca di conformità per cercare i messaggi. Per eliminare i messaggi, è necessario aggiungere il gruppo di ruoli Gestione organizzazione o il ruolo di gestione ricerca e Purge. Le autorizzazioni per questi ruoli vengono assegnate al [Centro sicurezza e conformità](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Creare una ricerca di contenuto](https://docs.microsoft.com/microsoft-365/compliance/content-search) per trovare il messaggio da eliminare.
- [Connettersi a PowerShell per Centro sicurezza e conformità](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Se si utilizza l'autenticazione a più fattori, vedere [Connect to Microsoft 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).