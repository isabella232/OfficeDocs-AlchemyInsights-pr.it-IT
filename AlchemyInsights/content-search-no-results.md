---
title: Ricerca contenuto nessun risultato
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680651"
---
# <a name="no-results-from-content-searchexports"></a>Nessun risultato dalla ricerca contenuto/esportazioni

Problemi relativi alla ricerca di contenuto/esportazioni la mancata restituzione di dati potrebbe essere dovuta a un determinato filtro di sicurezza di conformità che è stato configurato da un amministratore specifico e che non lo ha comunicato a tutti gli amministratori.

Per risolvere il problema, verificare se sono presenti filtri di sicurezza per la conformità che potrebbero causare questo problema:
1. Connettersi a PowerShell per Centro sicurezza e conformità
2. Eseguire le seguenti commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-Organization $org