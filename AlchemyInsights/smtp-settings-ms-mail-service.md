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
ms.openlocfilehash: e4d16a8d04b4d2fb4bfa8cf84308e29f2b499e0680f656cc239411d06e5b077c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900880"
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
 
Per informazioni sulle opzioni per l'inoltro della posta elettronica tramite Microsoft 365 e le procedure, vedere [Come configurare un dispositivo multifunzione o un'applicazione per l'invio di posta elettronica tramite Microsoft 365 o Office 365](https://docs.microsoft.com/exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).