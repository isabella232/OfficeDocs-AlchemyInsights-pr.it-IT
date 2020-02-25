---
title: Active Directory non sincronizzato
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265200"
---
# <a name="active-directory-not-syncing"></a>Active Directory non sincronizzato

Se si ricevono errori di sincronizzazione, ad esempio "Nessuna sincronizzazione recente" o si noterà che lo stato di sincronizzazione della directory nel portale di amministrazione di Office dice: "ultima sincronizzazione più di 3 giorni fa", potrebbe essere che AADConnect abbia impostazioni errate o insufficienti autorizzazioni per eseguire una sincronizzazione.  

La reinstallazione di AADConnect tramite le impostazioni di Express può risolvere il problema rapidamente:

1. [Scaricare la versione più recente di AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Seguire le istruzioni per l'installazione espressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Per ulteriori informazioni sugli account di servizio di AADConnect, vedere [Azure ad Connect: accounts and Permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
