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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028044"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Correzione del messaggio Microsoft 365 app "Spiacenti, un altro account dell'organizzazione è già connesso"

Per risolvere il problema, provare a eseguire le operazioni seguenti:

- Rimuovere tutti gli account di lavoro, ad eccezione dell'account interessato, Windows Impostazioni > **accesso all'istituto di istruzione o all'istituto di istruzione.**
- [Cancella Office credenziali usando](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) gestione Windows credenziali.<br/>
    **Nota:** I percorsi del Registro di Office 2016 sono stati modificati in 16.0. (Ad esempio: \Software\Microsoft\Office\16.0\Common\Identity\)
- Apri un app Office, scegli **File**  >  **Account**  >  **Disconnei**. Accedi quindi con un account utente con una licenza valida. Per informazioni dettagliate, vedere [Account in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Per Mac, vedere [Non è possibile accedere a un'app di Office 2016 per Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Per ulteriori informazioni, vedere "È già stato eseguito l'accesso a un altro account dell'organizzazione [nel computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).