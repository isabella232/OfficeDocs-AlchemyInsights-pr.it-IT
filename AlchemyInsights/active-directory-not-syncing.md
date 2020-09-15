---
title: Active Directory non sincronizzato
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697633"
---
# <a name="active-directory-not-syncing"></a>Active Directory non sincronizzato

Se si ricevono errori di sincronizzazione, ad esempio "Nessuna sincronizzazione recente" o si noterà che lo stato di sincronizzazione della directory nel portale di amministrazione di Office dice: "ultima sincronizzazione più di 3 giorni fa", potrebbe essere che AADConnect disponga di impostazioni errate o di autorizzazioni insufficienti per eseguire una sincronizzazione.  

La reinstallazione di AADConnect tramite le impostazioni di Express può risolvere il problema rapidamente:

1. [Scaricare la versione più recente di AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Seguire le istruzioni per l'installazione espressa](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Per altre informazioni sugli account dei servizi di AADConnect, vedere [Azure AD Connect: account e autorizzazioni](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
