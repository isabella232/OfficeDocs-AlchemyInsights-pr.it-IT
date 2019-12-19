---
title: Si è verificato un errore durante la convalida dell'errore del token di accesso durante la fase di analisi del desktop
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741208"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Errore durante la convalida del token di accesso" durante l'onboarding di analisi desktop

Questo errore viene generalmente osservato quando il token di autenticazione scade. In genere, l'aggiornamento della pagina Aggiorna il token. Tuttavia, questo problema può persistere se sono stati applicati criteri di accesso condizionale all'account utilizzato per l'analisi desktop di bordo. È possibile esaminare i registri di accesso di Azure AD nel portale di Azure per verificare se sono presenti errori di accesso per l'account utilizzato per l'onboarding di analisi desktop.

Per ulteriori informazioni sull'accesso condizionale, vedere [pianificare la distribuzione dell'accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).