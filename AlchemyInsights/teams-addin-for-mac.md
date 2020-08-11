---
title: Componente aggiuntivo Teams per Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/11/2020
ms.locfileid: "46617092"
---
# <a name="teams-add-in-for-mac"></a>Componente aggiuntivo Teams per Mac

Per risolvere i problemi relativi a un componente aggiuntivo mancante di Teams per Mac, segui questa procedura:

**Passaggio 1:** se hai Exchange ibrido locale (2016 CU3 o versione successiva), usa lo strumento Test-HMA.ps1 per confermare che l'autenticazione moderna ibrida è configurata correttamente. Per altre informazioni, vedere [Validare la configurazione dell'autenticazione moderna ibrida con Outlook per iOS e Android](https://aka.ms/AA980zq).  

**Nota:** utilizzare il formato di indirizzo UPN, ad esempio [username@contoso.com](mailto:username@contoso.com), non dominio\nomeutente. Eseguire questa operazione anche per gli utenti con cassette postali di Exchange Online.

**Passaggio 2:** Chiedere all'utente di andare in **Strumenti** > ** Account**... in Outlook per Mac, individuare e selezionare l'account. Verificare che il nome utente elencato sia in formato UPN, ad esempio [username@contoso.com](mailto:username@contoso.com).

**Passaggio 3:** Verificare che l'utente abbia una licenza di Microsoft Teams. L'utente deve usare l'abbonamento a Office 365 per Mac, prodotto versione 16.24 o successiva.