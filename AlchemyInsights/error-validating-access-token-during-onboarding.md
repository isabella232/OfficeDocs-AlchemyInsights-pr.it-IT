---
title: Errore durante la convalida del token di accesso durante l'on-boarding di Desktop Analytics
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
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946619"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Errore "Errore durante la convalida del token di accesso" durante l'onboarding di Desktop Analytics

Questo errore viene in genere rilevato alla scadenza del token di autenticazione. In genere, l'aggiornamento della pagina aggiorna il token. Tuttavia, questo problema può persistere se all'account utilizzato per l'on-board Desktop Analytics sono applicati criteri di accesso condizionale. È possibile esaminare i log di accesso di Azure AD nel portale di Azure per verificare se sono presenti errori di accesso per l'account utilizzato per l'onboarding di Desktop Analytics.

Per ulteriori informazioni sull'accesso condizionale, vedere [Plan your Conditional Access deployment.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)