---
title: Interfaccia di amministrazione di Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049348"
---
# <a name="teams-admin-center"></a>Interfaccia di amministrazione di Teams

Informazioni sulla gestione di Teams con l'[interfaccia di amministrazione di Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Se non si riesce ad accedere all'interfaccia di amministrazione di Teams, verificare quanto segue:

- Verificare di avere consentito [gli indirizzi IP e gli URL di Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) appropriati su tutti i dispositivi perimetrali (firewall e così via) o nelle regole firewall nel computer locale.
- Verificare che l'account usato per accedere al portale di amministrazione di Teams corrisponda al nome utente indicato nel [portale di amministrazione di Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Se gli utenti non sono visualizzati nell'interfaccia di amministrazione di Teams, verificare quanto segue:

- Sono stati creati utenti o sono state assegnate licenze nelle ultime 24 ore? Attendere almeno 24 ore prima di aprire un ticket di supporto.
- Sono state assegnate le licenze appropriate?
- Se si dispone di una directory di Active Directory locale, verificare che [il valore di msRTCSIP-PrimaryUserAddress o l'indirizzo SIP nel campo ProxyAddresses in Active Directory locale sia univoco e che il formato corrisponda al](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**Nome utente** dell'utente dall' [interfaccia di amministrazione di Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Se si prevede di mantenere una distribuzione di Skype for Business Server e di avere utenti locali e online: seguire le **"Configurazione ibrida con Teams e Skype for Business online"** nel pannello di controllo di Skype for Business Server e spostare gli utenti online.
