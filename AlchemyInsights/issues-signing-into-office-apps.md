---
title: Problemi di accesso alle Microsoft 365 app
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
- "9000571"
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986895"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Correzione del messaggio Microsoft 365 app "Il modulo Trusted Platform del computer non funziona correttamente"

Per risolvere il problema, provare a eseguire le operazioni seguenti:

- Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) [e Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Cancella Office credenziali usando](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) gestione Windows credenziali.<br/>
    **Nota:** I percorsi del Registro di Office 2016 sono stati modificati in 16.0. (Ad esempio: \Software\Microsoft\Office\16.0\Common\Identity\)
- Provare il [processo di ripristino degli](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) utenti per correggere gli errori TPM (Trusted Platform Module).
- Impostare EnableADAL = 0 seguendo la procedura seguente:  
    1. Fare clic con il pulsante Windows pulsante Start, scegliere **Esegui,** digitare **regedit** e quindi scegliere **OK.**
    2. Seleziona **Sì** per consentire all'editor del Registro di sistema di apportare modifiche al dispositivo.
    3. Nell'editor del Registro di sistema aggiungi un valore DWORD **EnableADAL** con un'impostazione pari a **0** in HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Per ulteriori informazioni, vedere [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).