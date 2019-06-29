---
title: Come abilitare SSO senza soluzione di continuità
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: d203c1256785a99426503a5386935d78f8966a8b
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384685"
---
# <a name="how-to-enable-seamless-sso"></a>Come abilitare SSO senza soluzione di continuità

Abilitare SSO trasparente tramite [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Se si sta eseguendo una nuova installazione di Azure AD Connect, scegliere il [percorso di installazione personalizzato](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). Nella pagina di **accesso dell'utente** , scegliere l'opzione **Abilita Single Sign-on** .
  
Per verificare la corretta abilitazione di SSO senza problemi:
  
1. Accedere al centro di [amministrazione di Azure Active Directory](https://aad.portal.azure.com) come amministratore globale.

2. Nel riquadro sinistro selezionare **Azure Active Directory** .

3. Verificare che l'accesso Single Sign-on sia **abilitato**.

Per ulteriori informazioni, vedere [Single Sign-on seamless di Azure Active Directory: Quick Start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  