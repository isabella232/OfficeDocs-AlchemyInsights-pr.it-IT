---
title: Configurare ed estendere la durata dei token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 97e89feda45439dae59acca5817fdf359623d647997d08a5cbe4a6314fa6db3a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044920"
---
# <a name="configure-and-extend-token-lifetimes"></a>Configurare ed estendere la durata dei token

È possibile specificare la durata di token di accesso, SAML o ID emesso da Microsoft Identity Platform. Inoltre, è possibile impostare la durata dei token per tutte le app dell'organizzazione, per un'applicazione multi-tenant (più organizzazioni) o per un'entità servizio specifica all'interno dell'organizzazione. Per altre informazioni, leggere [Durata dei token configurabile](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Per esempi, leggere [Esempi su come configurare la durata del token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Per informazioni su come configurare la durata e la compatibilità di un token in Azure Active Directory B2C (Azure AD B2C), vedere [Configurare token in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

L'articolo [Configurare il comportamento della sessione in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) descrive i metodi Single Sign-On (SSO) usati in Azure AD B2C e consente di scegliere il metodo SSO più appropriato per la configurazione dei criteri.

**Qual è la durata di un token? Per quanto tempo è valido?**

La durata di un token è di 1 ora, la durata di una sessione è di 24 ore. Ciò significa che se non vengono inviate richieste entro 24 ore, sarà necessario accedere di nuovo prima di richiedere un nuovo token.

> [!NOTE]
> A partire dal 30 maggio 2020, nessun nuovo tenant può usare i criteri di durata dei token configurabile per impostare i token della sessione e di aggiornamento. La deprecazione avverrà in diversi mesi, ciò significa che non verranno più rispettati i criteri dei token di sessione e di aggiornamento esistenti. È comunque possibile configurare la durata del token di accesso dopo la deprecazione.






