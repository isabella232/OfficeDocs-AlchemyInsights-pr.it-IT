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
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314208"
---
# <a name="active-directory-not-syncing"></a>Active Directory non sincronizzato

Se si ricevono errori di sincronizzazione, ad esempio "nessuna sincronizzazione recente" o si nota lo stato di sincronizzazione della directory nel portale di amministrazione di Office, "Ultima sincronizzazione più di 3 giorni fa", è possibile che AADConnect abbia impostazioni errate o autorizzazioni insufficienti per eseguire una sincronizzazione.  

La reinstallazione di AADConnect tramite impostazioni rapide potrebbe risolvere rapidamente il problema:

1. [Scaricare la versione più recente di AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Seguire le istruzioni per l'installazione rapida](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect deve essere installato in Windows Server 2012 o versione successiva. Il server deve essere aggiunto al dominio e può essere un controller di dominio o un server membro. Per un elenco completo dei requisiti Connessione azure AD e dei prerequisiti, vedere Prerequisiti per [Azure AD Connessione](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Per altre informazioni sugli account dei servizi di AADConnect, vedere [Azure AD Connect: account e autorizzazioni](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
