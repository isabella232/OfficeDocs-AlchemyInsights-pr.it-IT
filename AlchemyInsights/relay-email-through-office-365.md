---
title: Inoltrare la posta elettronica con Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ef06cfe41eee5d67bf82d4f64875ddafac82ee2062aade761f81b906cd428dd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024210"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Configurare un dispositivo multifunzione o un'applicazione per l'invio di posta elettronica

Per informazioni sulle opzioni e le procedure, vedere [Come configurare un dispositivo multifunzione o un'applicazione per l'invio di posta elettronica con Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Se di recente un dispositivo o un'applicazione ha smesso di funzionare, i motivi più comuni sono:

- **Errori correlati all'autenticazione durante l'utilizzo dell'invio del client di autenticazione SMTP**: di recente sono state apportate alcune modifiche relative al funzionamento dell'autenticazione SMTP. Per altre informazioni su come risolvere i problemi, vedere la sezione relativa alle autenticazioni non riuscite di [Risolvere i problemi relativi a stampanti, scanner e applicazioni line-of-business che inviano messaggi di posta elettronica tramite Microsoft 365 o Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).
- **Microsoft accetta solo la versione TLS 1.2 durante la connessione sicura a Office 365**: se si usa la connessione protetta (TLS), verificare che il dispositivo dell'applicazione supporti TLS 1.2. Per altre informazioni, vedere [Preparazione per TLS 1.2 in Office 365 e Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Per altri problemi e soluzioni, vedere [Risolvere i problemi relativi a stampanti, scanner e applicazioni line-of-business che inviano posta elettronica usando Microsoft 365 o Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).

Per vedere i dispositivi interessati, passare al [Report sui client di autenticazione SMTP](https://protection.office.com/mailflow/dashboard).

**Nota**: Exchange Online non supporta gli scenari di invio di posta elettronica in blocco. Per inviare messaggi di posta elettronica commerciali in blocco, ad esempio newsletter per i clienti, è necessario usare provider di terze parti specializzati per questi servizi.
