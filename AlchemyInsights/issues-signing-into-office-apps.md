---
title: Problemi di accesso alle app di Microsoft 365
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
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709110"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Correzione del messaggio "Il modulo piattaforma attendibile del computer non funziona correttamente" delle app di Microsoft 365

Per risolvere il problema, provare a eseguire le operazioni seguenti:

- Installare gli aggiornamenti più recenti per [Windows](https://support.microsoft.com/help/4027667/windows-10-update) e [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Cancellare le credenziali di Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) tramite Gestione credenziali di Windows.<br/>
    **Nota:** I percorsi del Registro di sistema per Office 2016 sono stati modificati in 16.0. (Ad esempio: \Software\Microsoft\Office\16.0\Common\Identity\)
- Provare il [processo di ripristino degli](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) utenti per correggere gli errori di Trusted Platform Module (TPM).
- Impostare EnableADAL = 0 seguendo la procedura seguente:  
    1. Fare clic con il pulsante destro del mouse sul pulsante Start di Windows, scegliere **Esegui,** digitare **regedit** e quindi scegliere **OK.**
    2. Seleziona **Sì** per consentire all'Editor del Registro di sistema di apportare modifiche al dispositivo.
    3. Nell'Editor del Registro di sistema aggiungi un valore DWORD **EnableADAL** con un'impostazione pari a **0** in HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Per ulteriori informazioni, vedere Problemi di connessione nell'accesso dopo l'aggiornamento a [Office 2016 build 16.0.7967 in Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)