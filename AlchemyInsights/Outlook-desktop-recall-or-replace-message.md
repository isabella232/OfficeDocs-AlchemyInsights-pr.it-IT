---
title: Outlook Richiamo del desktop o sostituzione di un messaggio di posta elettronica
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918399"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Richiamare o sostituire un messaggio Outlook di posta elettronica

- L'amministratore può richiamare **i messaggi per conto degli utenti tramite PowerShell.** Non è possibile richiamare i messaggi dall'interfaccia di amministrazione.
- È possibile **richiamare solo i messaggi inviati agli utenti dell'organizzazione.** Ad esempio, se il messaggio è stato inviato a un indirizzo Gmail, non è possibile richiamarlo.
- Puoi richiamare **solo i messaggi inviati da Outlook 2016 sul PC.** Se un utente invia un messaggio Outlook per Mac o Outlook sul web, non è possibile richiamarlo.

Per richiamare o sostituire un messaggio di posta elettronica:

1. Nel riquadro delle cartelle a sinistra della finestra Outlook, selezionare la cartella Posta inviata.
1. Fare doppio clic sul messaggio che si desidera richiamare per aprirlo.
1. Selezionare la **scheda** Messaggio e quindi selezionare **Azioni**  >  **Richiama questo messaggio**.
1. Selezionare **Elimina copie non lette del messaggio** o Elimina copie non **lette** e sostituisci con un nuovo messaggio e quindi selezionare **OK.**
1. Se si sta inviando un messaggio sostitutivo, comporre il messaggio e quindi selezionare **Invia**.
1. L'esito positivo o negativo del richiamo di un messaggio dipende dalle impostazioni del destinatario in Outlook. Per la procedura per controllare il richiamo, vedi [questo articolo.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Cercare ed eliminare messaggi di posta elettronica nell'organizzazione

- Se non si è un amministratore globale, l'account deve essere aggiunto al ruolo Responsabile eDiscovery o al ruolo di gestione ricerca di conformità per cercare i messaggi. Per eliminare i messaggi, è necessario aggiungere il gruppo di ruoli Gestione organizzazione o il ruolo di gestione Ricerca ed eliminazione. Le autorizzazioni per questi ruoli vengono assegnate nel [Centro sicurezza e conformità.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Creare una ricerca di contenuto](https://docs.microsoft.com/microsoft-365/compliance/content-search) per trovare il messaggio da eliminare.
- [Connessione a PowerShell per Centro sicurezza e conformità.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Se si usa l'autenticazione a più fattori, vedere Connessione per Microsoft 365 sicurezza e Centro conformità [PowerShell con l'autenticazione a più fattori.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)