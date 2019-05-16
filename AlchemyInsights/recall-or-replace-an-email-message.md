---
title: Richiamare o sostituire un messaggio di posta elettronica
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1860
ms.assetid: ''
ms.openlocfilehash: 6e66b5d60fe9ac66c2f2f8f7e99e753652c3a59e
ms.sourcegitcommit: bcb2612ab8ba2aee5165e3912dca95cc1bdd09f4
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 05/16/2019
ms.locfileid: "34096542"
---
# <a name="recall-or-replace-an-email-message"></a>Richiamare o sostituire un messaggio di posta elettronica

- È possibile **richiamare solo i messaggi inviati alle persone all'interno dell'organizzazione**. Se il messaggio è stato inviato a un indirizzo Gmail, ad esempio, non è possibile richiamarlo.
- È possibile **richiamare solo i messaggi inviati da Outlook 2016 per il PC**. Se un utente invia un messaggio utilizzando Outlook per Mac o Outlook sul Web, non è possibile richiamarlo.
- Se si è un amministratore, è possibile **richiamare i messaggi per conto degli utenti utilizzando PowerShell**. Non è possibile richiamare messaggi dall'interfaccia di amministrazione. Scorrere verso il basso fino a "cercare ed eliminare i messaggi di posta elettronica nell'organizzazione" per ulteriori informazioni.

***Richiamare o sostituire un messaggio di posta elettronica inviato***
1. Nel riquadro delle cartelle nella parte sinistra della finestra di Outlook scegliere la cartella posta inviata.
2. Aprire il messaggio che si desidera richiamare. È necessario fare doppio clic per aprire il messaggio. Se si seleziona il messaggio in modo che venga visualizzato nel riquadro di lettura, non sarà possibile richiamare il messaggio.
3. Nella scheda messaggio, selezionare **azioni** > **richiamare questo messaggio**.
4. Scegliere **Elimina copie non lette del messaggio** o **Elimina copie non lette e Sostituisci con un nuovo messaggio**, quindi selezionare **OK**.
5. Se si sta inviando un messaggio di sostituzione, comporre il messaggio, quindi selezionare **Invia**.
6. L'esito positivo o negativo di un messaggio di richiamo dipende dalle impostazioni dei destinatari in Outlook. 

Per ulteriori informazioni, tra cui la verifica del richiamo, vedere [Recall or Replace an email message you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Cercare ed eliminare i messaggi di posta elettronica nell'organizzazione*** Per cercare ed eliminare i messaggi di posta elettronica nell'organizzazione, è più semplice se si è un amministratore globale. Se non si è un amministratore globale, è necessario aggiungere l'account al gruppo di ruoli di eDiscovery Manager o al ruolo di gestione della ricerca di conformità. Per eliminare i messaggi, è necessario aggiungere il gruppo di ruoli Gestione organizzazione o il ruolo di gestione ricerca e Purge. Le autorizzazioni per questi ruoli sono assegnate al [Centro sicurezza & Compliance](https://protection.office.com/).

1. [Creare una ricerca di contenuto](https://docs.microsoft.com/en-us/office365/securitycompliance/content-search) per trovare il messaggio da eliminare.
2. [Connettersi a PowerShell per Centro sicurezza _AMP_ Compliance](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Se si utilizza l'autenticazione Master, vedere [Connect to Office 365 Security _AMP_ Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/en-us/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 