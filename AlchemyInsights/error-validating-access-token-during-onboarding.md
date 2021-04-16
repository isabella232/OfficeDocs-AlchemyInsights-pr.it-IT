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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813692"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Errore "Errore durante la convalida del token di accesso" durante l'onboarding di Desktop Analytics

Questo errore viene in genere rilevato alla scadenza del token di autenticazione. In genere, l'aggiornamento della pagina aggiorna il token. Tuttavia, questo problema può persistere se all'account utilizzato per l'on-board Desktop Analytics sono applicati criteri di accesso condizionale. È possibile esaminare i log di accesso di Azure AD nel portale di Azure per verificare se sono presenti errori di accesso per l'account utilizzato per l'onboarding di Desktop Analytics.

Per ulteriori informazioni sull'accesso condizionale, vedere [Plan your Conditional Access deployment.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)