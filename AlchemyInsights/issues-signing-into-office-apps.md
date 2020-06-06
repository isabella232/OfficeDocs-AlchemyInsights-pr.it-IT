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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579869"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Risoluzione delle app Microsoft 365 "il modulo della piattaforma trusted del computer non funziona correttamente" messaggio

Per risolvere il problema, provare a eseguire le operazioni seguenti:

- Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Cancellare le credenziali di Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) utilizzando Gestione credenziali di Windows.<br/>
    **Nota:** I percorsi del registro di sistema per Office 2016 sono stati modificati in 16,0. (Es: \Software\Microsoft\Office\16.0\Common\Identity\)
- Provare a eseguire il [processo di ripristino dell'utente](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) per correggere gli errori TPM (Trusted Platform Module).
- Impostare EnableADAL = 0 eseguendo la procedura seguente:  
    1. Fare clic con il pulsante destro del mouse su Start, scegliere **Esegui**, digitare **Regedit**e quindi scegliere **OK**.
    2. Selezionare **Sì** per consentire all'editor del registro di sistema di apportare modifiche al dispositivo.
    3. Nell'editor del registro di sistema aggiungere un valore DWORD di **EnableADAL** con un'impostazione pari a **0** in HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Per ulteriori informazioni, vedere [Connection issues in Sign-in after update to Office 2016 Build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).