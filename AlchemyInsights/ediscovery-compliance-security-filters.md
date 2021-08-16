---
title: Nessun risultato restituito durante ricerca/esportazione contenuto
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101270"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nessun risultato restituito durante ricerca/esportazione contenuto

Se si verificano problemi con i seguenti scenari di eDiscovery:

- Ricerca/esportazione contenuto non restituisce dati o dati imprevisti
- Ricerca o esportazione di eDiscovery non riesce

Ciò può essere dovuto a determinati filtri di sicurezza della conformità che sono stati configurazione da un amministratore specifico e non sono stati comunicati a tutti gli amministratori.

Per risolvere il problema, verificare se sono presenti filtri di sicurezza di conformità che potrebbero causare questi problemi:

1. Connessione powershell per centro sicurezza e conformità
2. Eseguire i seguenti commandlet:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Per ulteriori informazioni sui filtri di sicurezza di conformità, vedere [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
