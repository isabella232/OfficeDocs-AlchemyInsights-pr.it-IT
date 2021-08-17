---
title: Ricerca contenuto Nessun risultato
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
- "9000661"
- "2527"
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058006"
---
# <a name="no-results-from-content-searchexports"></a>Nessun risultato da Ricerca/Esportazioni contenuto

I problemi relativi alla ricerca/esportazione del contenuto che non restituiscono dati potrebbero essere dovuti a determinati filtri di sicurezza della conformità che sono stati impostati da un amministratore specifico e che non lo comunicano a tutti gli amministratori.

Per risolvere il problema, verificare se sono presenti filtri di sicurezza di conformità che potrebbero causare questo problema:
1. Connessione powershell per centro sicurezza e conformità
2. Eseguire i seguenti commandlet:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org