---
title: Nessun risultato restituito durante la ricerca di contenuto/esportazione
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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666651"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nessun risultato restituito durante la ricerca di contenuto/esportazione

Se si verificano problemi con gli scenari di eDiscovery seguenti:

- Ricerca contenuto/Esporta non restituisce dati o dati imprevisti
- errore di ricerca o esportazione di eDiscovery

Questo può essere dovuto a determinati filtri di sicurezza di conformità che sono stati impostati da un amministratore specifico e non sono stati comunicati a tutti gli amministratori.

Per risolvere il problema, controllare se sono presenti filtri di sicurezza per la conformità che potrebbero causare questi problemi:

1. Connettersi a PowerShell per Centro sicurezza e conformità
2. Eseguire le seguenti commandlets:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Per ulteriori informazioni sui filtri di sicurezza di conformità, vedere [filtro delle autorizzazioni per la ricerca di contenuto](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
