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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098606"
---
# <a name="issues-with-azure-mfa"></a>Problemi con Azure MFA
Ci sono un paio di cose da verificare se gli utenti non possono accedere usando l'autenticazione a più fattori (MFA)

1. L'utente interessato potrebbe essere bloccato in Azure Active Directory Portal. In questo caso, i tentativi di autenticazione per l'utente specifico verranno automaticamente negati. [Segui i passaggi descritti in questo articolo per sbloccarli.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se lo sblocco dell'utente non è stato utile o l'utente non è bloccato, puoi provare a reimpostare la MFA per l'utente e l'utente dovrà ripetere il processo di registrazione. [Seguire i passaggi descritti in questo articolo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se questa è la prima volta che è stata abilitata l'autenticazione a più fattori e gli utenti non sono in grado di accedere a client non browser come Outlook, Skype e così via, ad esempio ADAL (Active Directory Authentication Library) non è abilitato nell'abbonamento a O365. In questo caso sarà necessario connettersi Exchange Online PowerShell ed eseguire questo cmdlet: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*