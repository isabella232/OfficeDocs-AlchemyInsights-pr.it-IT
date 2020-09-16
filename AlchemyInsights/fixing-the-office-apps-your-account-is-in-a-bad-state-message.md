---
title: Risoluzione delle app di Microsoft 365 l'account è in un messaggio di stato non valido
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744549"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Risoluzione dei problemi relativi a Microsoft 365 Apps "l'account è in uno stato non corretto"

Per correggere l'errore, provare a eseguire le opzioni seguenti nel computer in questione:

- Aprire un'app di Office, **File**selezionare l'  >  **account**  >  **di accesso al file fuori da tutti gli account**. Eseguire nuovamente l'accesso usando un account utente con una licenza valida. Per informazioni dettagliate, vedere [Account in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.<br>
  **Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0. Ad esempio, \Software\Microsoft\Office\16.0\Common\Identity\
- Se si verifica un errore durante la connessione a Office 365 con Office 2013, [abilitare l'autenticazione moderna](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) per il client di Office.

Per ulteriori informazioni, vedere [come risolvere i problemi relativi alle app non browser che non sono in grado di accedere a Microsoft 365, Azure o Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

