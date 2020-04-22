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
ms.openlocfilehash: ac760b417ad98b9d5bb6be4b92e60074ab93ceb3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43708691"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Errore di correzione delle app di Office "l'account è in uno stato non valido"

Per correggere l'errore, provare a eseguire le opzioni seguenti nel computer in questione:

- Aprire un'app di Office, **File** > Selezionare l'**account** > **di accesso al file fuori da tutti gli account**. Eseguire di nuovo l'accesso utilizzando un account utente con una licenza valida. Per informazioni dettagliate, vedere [Account in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.<br>
  **Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0. Ad esempio, \Software\Microsoft\Office\16.0\Common\Identity\
- Se si verifica un errore durante la connessione a Office 365 con Office 2013, [abilitare l'autenticazione moderna](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) per il client di Office.

Per ulteriori informazioni, vedere [come risolvere i problemi relativi alle app non browser che non sono in grado di accedere a Microsoft 365, Azure o Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

