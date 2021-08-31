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
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744650"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemi di accesso Microsoft 365 Apps

Nota: se si utilizza una versione precedente di Windows (ad esempio Windows 7 SP1, Windows Server 2008 R2), utilizzare la correzione semplice per abilitare TLS 1.2 come predefinito. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Per ulteriori informazioni, vedere [Aggiornamento per abilitare TLS 1.1 e TLS 1.2 come protocollo di protezione predefinito in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).

Per risolvere i problemi di accesso con le app di Microsoft 365, provare le opzioni seguenti nel computer interessato:  

- Per Windows, [vedere Consigli sulla risoluzione dei problemi di accesso comuni](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Per Mac, vedi [Can't sign in to an Office 2016 per Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Suggerimento:** nei computer Windows è possibile diagnosticare e risolvere automaticamente diversi problemi comuni di accesso a Office. Scaricare ed eseguire l'**[Assistente supporto e ripristino di Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** per usare il tool automatizzato.

**Nota:** Non è consigliabile disabilitare l'autenticazione moderna (ADAL) o wam (Web Account Management) per risolvere i problemi di accesso o **attivazione.** Se gli errori si verificano durante la connessione a Microsoft 365 utilizzando Office [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) 2013, assicurarsi di abilitare l'autenticazione moderna per Office client.

Per azioni di risoluzione dei problemi specifiche, vedere:

[Problemi di connessione durante l'accesso dopo l'aggiornamento a Office 2016 build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Non è possibile accedere all'account dell'organizzazione, ad esempio Office 365, Azure o Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Come risolvere i problemi delle app non browser che non possono accedere a Office 365, Azure o Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Ripetutamente richiesto di immettere le credenziali in Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)