---
title: Si è verificato un errore durante la convalida dell'errore del token di accesso durante la fase di analisi del desktop
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783555"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>"Errore durante la convalida del token di accesso" durante l'onboarding di analisi desktop

Questo errore viene generalmente osservato quando il token di autenticazione scade. In genere, l'aggiornamento della pagina Aggiorna il token. Tuttavia, questo problema può persistere se sono stati applicati criteri di accesso condizionale all'account utilizzato per l'analisi desktop di bordo. È possibile esaminare i registri di accesso di Azure AD nel portale di Azure per verificare se sono presenti errori di accesso per l'account utilizzato per l'onboarding di analisi desktop.

Per ulteriori informazioni sull'accesso condizionale, vedere [pianificare la distribuzione dell'accesso condizionale](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).