---
title: Correzione delle app di Microsoft 365 L'account è in un messaggio di stato non valido
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
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812540"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Correzione dell'errore "L'account è in uno stato non valido" delle app di Microsoft 365

Per correggere l'errore, provare le opzioni seguenti nel computer interessato:

- Apri un'app di Office, seleziona **File**  >  **Account**  >  **Disconnei da tutti gli account**. Eseguire nuovamente l'accesso usando un account utente con una licenza valida. Per informazioni dettagliate, vedere [Account in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) tramite Gestione credenziali di Windows.<br>
  **Nota:** I percorsi del Registro di sistema per Office 2016 sono stati modificati in 16.0. Ad esempio, \Software\Microsoft\Office\16.0\Common\Identity\
- Se l'errore si verifica durante la connessione a Office 365 con Office 2013, abilitare l'autenticazione [moderna](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) per il client di Office.

Per altre informazioni, vedi Come risolvere i problemi relativi alle app non browser che non possono accedere [a Microsoft 365, Azure o Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)

