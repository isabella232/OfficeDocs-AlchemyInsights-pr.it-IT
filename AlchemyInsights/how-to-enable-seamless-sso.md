---
title: Come abilitare SSO senza soluzione di continuità
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
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780531"
---
# <a name="how-to-enable-seamless-sso"></a>Come abilitare SSO senza soluzione di continuità

Abilitare SSO trasparente tramite [Azure ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).
  
Se si sta eseguendo una nuova installazione di Azure AD Connect, scegliere il [percorso di installazione personalizzato](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom). Nella pagina di **accesso dell'utente** , scegliere l'opzione **Abilita Single Sign-on** .
  
Per verificare la corretta abilitazione di SSO senza problemi:
  
1. Accedere al centro di [amministrazione di Azure Active Directory](https://aad.portal.azure.com) come amministratore globale.

2. Nel riquadro sinistro selezionare **Azure Active Directory** .

3. Verificare che l'accesso Single Sign-on sia **abilitato**.

Per ulteriori informazioni, vedere [Single Sign-on seamless di Azure Active Directory: Quick Start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).
  