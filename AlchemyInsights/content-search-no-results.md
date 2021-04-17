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
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816852"
---
# <a name="no-results-from-content-searchexports"></a>Nessun risultato da Ricerca/Esportazioni contenuto

I problemi relativi alla ricerca/esportazione del contenuto che non restituiscono dati potrebbero essere dovuti a determinati filtri di sicurezza della conformità che sono stati impostati da un amministratore specifico e che non lo comunicano a tutti gli amministratori.

Per risolvere il problema, verificare se sono presenti filtri di sicurezza di conformità che potrebbero causare questo problema:
1. Connettersi a Powershell per Centro sicurezza e conformità
2. Eseguire i seguenti commandlet:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org