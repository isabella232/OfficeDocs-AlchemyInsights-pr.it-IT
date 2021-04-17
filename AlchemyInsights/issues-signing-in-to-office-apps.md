---
title: Problemi di accesso alle app di Microsoft 365
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
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833079"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Correzione delle app di Microsoft 365 "Spiacenti, un altro account dell'organizzazione è già connesso"

Per risolvere il problema, provare a eseguire le operazioni seguenti:

- Rimuovi tutti gli account di lavoro, ad eccezione dell'account interessato, usando Impostazioni di Windows > **Accedi all'istituto di istruzione o all'istituto di istruzione.**
- [Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) tramite Gestione credenziali di Windows.<br/>
    **Nota:** I percorsi del Registro di sistema per Office 2016 sono stati modificati in 16.0. (Ad esempio: \Software\Microsoft\Office\16.0\Common\Identity\)
- Apri un'app di Office, scegli **File**  >  **Account**  >  **Disconnei**. Accedi quindi con un account utente con una licenza valida. Per informazioni dettagliate, vedere [Account in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Per Mac, vedere [Non è possibile accedere a un'app di Office 2016 per Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Per ulteriori informazioni, vedere "È già stato eseguito l'accesso a un altro account dell'organizzazione [in questo computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).