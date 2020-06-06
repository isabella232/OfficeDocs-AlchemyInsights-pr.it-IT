---
title: Problemi di accesso a Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579941"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Risoluzione delle app Microsoft 365 "spiacenti, un altro account dell'organizzazione è già stato firmato in" messaggio

Per risolvere il problema, provare a eseguire le operazioni seguenti:

- Rimuovere tutti gli account di lavoro, ad eccezione dell'account danneggiato, utilizzando le impostazioni di Windows > **accedere al lavoro o all'Istituto di istruzione**.
- [Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.<br/>
    **Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0. (Es: \Software\Microsoft\Office\16.0\Common\Identity\)
- Aprire un'app di Office, **File**scegliere  >  **Account**  >  **Esci dall'** account file. Accedere quindi utilizzando un account utente con una licenza valida. Per informazioni dettagliate, vedere [Account in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Per Mac, vedere [Non è possibile accedere a un'app di Office 2016 per Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Per ulteriori informazioni, vedere [la sezione "spiacenti, un altro account dell'organizzazione è già stato eseguito l'accesso a questo computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).