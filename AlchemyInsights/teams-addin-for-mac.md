---
title: Componente aggiuntivo Teams per Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670332"
---
# <a name="teams-add-in-for-mac"></a>Componente aggiuntivo Teams per Mac

Per risolvere i problemi relativi a un componente aggiuntivo mancante di Teams per Mac, segui questa procedura:

**Passaggio 1:** se hai Exchange ibrido locale (2016 CU3 o versione successiva), usa lo strumento Test-HMA.ps1 per confermare che l'autenticazione moderna ibrida è configurata correttamente. Per altre informazioni, vedere [Validare la configurazione dell'autenticazione moderna ibrida con Outlook per iOS e Android](https://aka.ms/AA980zq).  

**Nota:** utilizzare il formato di indirizzo UPN, ad esempio [username@contoso.com](mailto:username@contoso.com), non dominio\nomeutente. Eseguire questa operazione anche per gli utenti con cassette postali di Exchange Online.

**Passaggio 2:** Chiedere all'utente di andare in **Strumenti** > ** Account**... in Outlook per Mac, individuare e selezionare l'account. Verificare che il nome utente elencato sia in formato UPN, ad esempio [username@contoso.com](mailto:username@contoso.com).

**Passaggio 3:** Verificare che l'utente abbia una licenza di Microsoft Teams. L'utente deve usare l'abbonamento a Office 365 per Mac, prodotto versione 16.24 o successiva.