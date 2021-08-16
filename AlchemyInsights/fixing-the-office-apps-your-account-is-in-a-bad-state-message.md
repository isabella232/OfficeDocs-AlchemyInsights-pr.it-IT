---
title: Correzione delle app Microsoft 365 il tuo account è in un messaggio di stato non valido
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
- "2558"
- "9000571"
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068240"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Correzione dell'errore Microsoft 365 app "Il tuo account è in uno stato non valido"

Per correggere l'errore, provare le opzioni seguenti nel computer interessato:

- Apri un app Office, seleziona **File**  >  **Account**  >  **Disconnei da tutti gli account.** Eseguire nuovamente l'accesso usando un account utente con una licenza valida. Per informazioni dettagliate, vedere [Account in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Cancella Office credenziali usando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) gestione Windows credenziali.<br>
  **Nota:** I percorsi del Registro di Office 2016 sono stati modificati in 16.0. Ad esempio, \Software\Microsoft\Office\16.0\Common\Identity\
- Se l'errore si verifica durante la connessione a Office 365 utilizzando [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) Office 2013, abilitare l'autenticazione moderna per il client Office client.

Per altre informazioni, vedi Come risolvere i problemi relativi alle app non browser che non possono accedere [a Microsoft 365, Azure o Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

