---
title: Risolvere i problemi di autenticazione SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737993"
---
# <a name="solving-smtp-authentication-issues"></a>Risolvere i problemi di autenticazione SMTP

Se si verificano gli errori 5.7.57 o 5.7.3 quando si prova a inviare posta elettronica SMTP ed eseguire l'autenticazione con un client o un'applicazione, è necessario verificare alcuni aspetti:

- L'invio SMTP autenticato potrebbe essere disabilitato nel tenant o nella cassetta postale che si sta provando a usare (controllare entrambe le impostazioni). Per altre informazioni, vedere [Abilitare o disabilitare l'invio SMTP client autenticato](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Controllare se per il tenant sono abilitate le [Impostazioni predefinite per la sicurezza di Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). Se abilitate, l'autenticazione SMTP mediante autenticazione di base, nota anche come legacy, che usa il nome utente e la password, non riuscirà.
