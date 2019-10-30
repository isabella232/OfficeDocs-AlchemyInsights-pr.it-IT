---
title: Problemi con AMF
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768841"
---
# <a name="issues-with-azure-mfa"></a>Problemi con Azure AMF
È possibile verificare se gli utenti non possono eseguire l'accesso utilizzando l'autenticazione a più fattori (AMF)

1. L'utente può essere bloccato nel portale di Azure Active Directory. In caso contrario, i tentativi di autenticazione per l'utente specifico verranno negati automaticamente. [Attenersi alla procedura descritta in questo articolo per sbloccarli.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Se lo sblocco dell'utente non è stato di aiuto o se l'utente non è bloccato, è possibile provare a reimpostare AMF per l'utente e il processo di registrazione passerà di nuovo. [Seguire le istruzioni riportate in questo articolo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Se è la prima volta che si Abilita l'autenticazione master e gli utenti non sono in grado di accedere ai client non browser come Outlook, Skype e così via, è possibile che ADAL (Active Directory Authentication Library) non sia abilitato per l'abbonamento a O365. In questo caso, sarà necessario connettersi a PowerShell di Exchange Online ed eseguire questo cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*