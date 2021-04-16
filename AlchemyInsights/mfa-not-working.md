---
title: Problemi con MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810488"
---
# <a name="issues-with-azure-mfa"></a>Problemi con Azure MFA
Ci sono un paio di cose da verificare se gli utenti non possono accedere usando l'autenticazione a più fattori (MFA)

1. L'utente interessato potrebbe essere bloccato nel portale di Azure Active Directory. In questo caso, i tentativi di autenticazione per l'utente specifico verranno automaticamente negati. [Segui i passaggi descritti in questo articolo per sbloccarli.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se lo sblocco dell'utente non è stato utile o l'utente non è bloccato, puoi provare a reimpostare la MFA per l'utente e l'utente dovrà ripetere il processo di registrazione. [Seguire i passaggi descritti in questo articolo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se questa è la prima volta che hai abilitato L'autenticazione a più fattori e gli utenti non sono in grado di accedere a client non browser come Outlook, Skype e così via, ad esempio ADAL (Active Directory Authentication Library) non è abilitato nell'abbonamento a O365. In questo caso sarà necessario connettersi a PowerShell di Exchange Online ed eseguire questo cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*