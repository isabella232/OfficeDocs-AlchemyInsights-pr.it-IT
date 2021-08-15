---
title: Richiamare o sostituire un messaggio di posta elettronica
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024390"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Richiamare o sostituire un messaggio di posta elettronica in Microsoft 365

- È possibile **richiamare solo i messaggi inviati agli utenti dell'organizzazione.** Ad esempio, se il messaggio è stato inviato a un indirizzo Gmail, non è possibile richiamarlo.
- È possibile **richiamare solo i messaggi inviati da Outlook per il PC.** Se un utente invia un messaggio Outlook per Mac o Outlook sul web, non è possibile richiamarlo.
- In quanto amministratore tenant, è possibile richiamare i messaggi per conto degli utenti tramite **PowerShell** (per ulteriori informazioni, vedere: [Cercare ed eliminare i messaggi di posta elettronica](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Non è possibile richiamare i messaggi dall'interfaccia di amministrazione. Scorrere verso il basso fino a "Cercare ed eliminare i messaggi di posta elettronica nell'organizzazione" per ulteriori informazioni.

**Richiamare o sostituire un messaggio di posta elettronica inviato**

1. Nel riquadro delle cartelle a sinistra della finestra Outlook, scegliere la cartella Posta inviata.
2. Aprire il messaggio che si desidera richiamare. È necessario fare doppio clic per aprire il messaggio. Se si seleziona il messaggio in modo che venga visualizzato nel riquadro di lettura, non sarà possibile richiamare il messaggio.
3. Nella scheda Messaggio selezionare **Azioni**  >  **Richiama questo messaggio**.
4. Scegliere **Elimina copie non lette del messaggio** oppure Elimina copie non **lette** e sostituisci con un nuovo messaggio, quindi selezionare **OK.**
5. Se si sta inviando un messaggio sostitutivo, comporre il messaggio, quindi selezionare **Invia**.
6. L'esito positivo o negativo del richiamo di un messaggio dipende dalle impostazioni dei destinatari in Outlook.

Per ulteriori informazioni, inclusa la modalità di controllo del richiamo, vedere Richiamare o sostituire un messaggio di posta [elettronica inviato.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Per cercare ed eliminare i messaggi di posta*** elettronica nell'organizzazione, è più semplice se si è un amministratore globale. Se non si è un amministratore globale, l'account deve essere aggiunto al gruppo di ruoli Manager eDiscovery o al ruolo di gestione ricerca di conformità. Per eliminare i messaggi, è necessario aggiungere il gruppo di ruoli Gestione organizzazione o il ruolo di gestione Ricerca ed eliminazione. Le autorizzazioni per questi ruoli vengono assegnate nel [Centro sicurezza & conformità](https://protection.office.com/).

1. [Creare una ricerca di contenuto](https://docs.microsoft.com/microsoft-365/compliance/content-search) per trovare il messaggio da eliminare.
2. [Connettersi a PowerShell in Centro sicurezza e conformità](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Se si usa MFA (autenticazione a più fattori), vedere Connessione [to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
