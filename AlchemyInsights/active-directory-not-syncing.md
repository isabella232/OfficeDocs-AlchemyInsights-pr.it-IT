---
title: Active Directory non sincronizzato
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937105"
---
# <a name="active-directory-not-syncing"></a>Active Directory non sincronizzato

Se si ricevono errori di sincronizzazione, ad esempio "nessuna sincronizzazione recente" o si nota lo stato di sincronizzazione della directory nel portale di amministrazione di Office, "Ultima sincronizzazione più di 3 giorni fa", è possibile che AADConnect abbia impostazioni errate o autorizzazioni insufficienti per eseguire una sincronizzazione.  

La reinstallazione di AADConnect tramite impostazioni rapide potrebbe risolvere rapidamente il problema:

1. [Scaricare la versione più recente di AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Seguire le istruzioni per l'installazione rapida](/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect deve essere installato in Windows Server 2012 o versione successiva. Il server deve essere aggiunto al dominio e può essere un controller di dominio o un server membro. Per un elenco completo dei requisiti Connessione azure AD e dei prerequisiti, vedere [Prerequisiti per Azure AD Connessione](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Per altre informazioni sugli account dei servizi di AADConnect, vedere [Azure AD Connect: account e autorizzazioni](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
