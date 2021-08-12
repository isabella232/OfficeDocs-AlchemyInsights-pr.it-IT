---
title: Impostazioni SMTP per il servizio di posta di Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12073"
- "3000003"
ms.openlocfilehash: 261695a0bf736a51514df50c0ad66aaab5b50edb
ms.sourcegitcommit: e9fcd72e64d35f5ba14dfa0fbde39eae20d86cfe
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/27/2021
ms.locfileid: "53603297"
---
# <a name="smtp-settings-for-the-microsoft-365-mail-service"></a>Impostazioni SMTP per il servizio di posta di Microsoft 365

Queste sono le impostazioni SMTP per i servizi di posta di Microsoft 365:

**Server**: smtp.office365.com </br>
**Porta:** 587 </br>
**Crittografia**: STARTTLS (ora è supportata solo la versione TLS 1.2. Assicurarsi che l'applicazione o il dispositivo supporti la versione TLS 1.2) </br>
**Nome utente**: l'indirizzo di Office 365 (ad esempio example@yourdomain.com) </br>
**Password**: la password di Office 365 </br>
**Autenticazione**: necessaria </br>
**Limiti di invio**: 10.000 messaggi di posta elettronica al giorno </br>

Per le impostazioni POP e IMAP, vedere [Impostazioni POP, IMAP e SMTP](https://support.microsoft.com/office/pop-imap-and-smtp-settings-8361e398-8af4-4e97-b147-6c6c4ac95353).
 
Per informazioni sulle opzioni per l'inoltro della posta elettronica tramite Microsoft 365 e le procedure, vedere [Come configurare un dispositivo multifunzione o un'applicazione per l'invio di posta elettronica tramite Microsoft 365 o Office 365](/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).