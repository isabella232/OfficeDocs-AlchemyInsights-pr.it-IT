---
title: Risoluzione delle app di Office l'account è in un messaggio di stato non valido
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969561"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Errore di correzione delle app di Office "l'account è in uno stato non valido"

Per correggere l'errore, provare a eseguire le opzioni seguenti nel computer in questione:

- Aprire un'app di Office, **** > Selezionare l'**account** > **di accesso al file fuori da tutti gli account**. Eseguire di nuovo l'accesso utilizzando un account utente con una licenza valida. Per informazioni dettagliate, vedere [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.<br>
  **Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0. Ad esempio, \Software\Microsoft\Office\16.0\Common\Identity\
- Nel computer in questione, impostare EnableADAL = 0 eseguendo la procedura seguente:  
     1. Fare clic con il pulsante destro del mouse su Windows e scegliere **Esegui**. Nella casella **Apri** Digitare **Regedit**e quindi fare clic su **OK**.
     2. Selezionare **Sì** quando viene richiesto di consentire all'editor del registro di sistema di apportare modifiche al dispositivo.
    3. Nell'editor del registro di sistema, aggiungere un valore DWORD di EnableADAL con un'impostazione pari a 0 in HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Se si verifica un errore durante la connessione a Office 365 con Office 2013, [abilitare l'autenticazione moderna](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) per il client di Office.

Per ulteriori informazioni, vedere [come risolvere i problemi relativi alle app non browser che non sono in grado di accedere a Office 365, Azure o Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

