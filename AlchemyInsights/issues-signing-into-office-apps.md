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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833007"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Correzione delle app di Microsoft 365 "Il modulo Trusted Platform del computer non funziona correttamente"

Per risolvere il problema, provare a eseguire le operazioni seguenti:

- Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) tramite Gestione credenziali di Windows.<br/>
    **Nota:** I percorsi del Registro di sistema per Office 2016 sono stati modificati in 16.0. (Ad esempio: \Software\Microsoft\Office\16.0\Common\Identity\)
- Provare il [processo di ripristino degli](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) utenti per correggere gli errori TPM (Trusted Platform Module).
- Impostare EnableADAL = 0 seguendo la procedura seguente:  
    1. Fai clic con il pulsante destro del mouse sul pulsante Start di Windows, scegli **Esegui,** digita **regedit** e quindi scegli **OK.**
    2. Seleziona **Sì** per consentire all'editor del Registro di sistema di apportare modifiche al dispositivo.
    3. Nell'editor del Registro di sistema aggiungi un valore DWORD **EnableADAL** con un'impostazione pari a **0** in HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Per ulteriori informazioni, vedere [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)