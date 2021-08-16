---
title: Problemi relativi alle attestazioni e agli attributi dei token
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012888"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemi relativi alle attestazioni e agli attributi dei token

**Aggiornare, configurare o rimuovere attestazioni token**

1. Usando Azure Active Directory (Azure AD), è [](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) possibile personalizzare il tipo di attestazione per l'attestazione di ruolo nel token di risposta ricevuto dopo l'autorizzazione di un'app.
2. Gli sviluppatori di applicazioni possono usare attestazioni facoltative nelle applicazioni azure AD per specificare le attestazioni desiderate nei token inviati all'applicazione. Per altre informazioni, vedi [Fornire attestazioni facoltative per la tua app.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Configurare le attestazioni di gruppo per le applicazioni con Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Se si usa l'accesso Single #A0 nell'applicazione, vedere personalizzare le attestazioni [emesse](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)nel token SAML per le applicazioni aziendali.

**Mapping degli attributi delle attestazioni**

1. Per configurare i criteri di mapping delle attestazioni tramite PowerShell, vedere Personalizzare le attestazioni emesse nei token per [un'app specifica in un tenant (anteprima).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. Gli attributi dell'estensione dello schema di directory consentono di archiviare dati aggiuntivi in Azure Active Directory oggetti utente e altri oggetti directory, ad esempio gruppi, dettagli del tenant, entità servizio. Solo gli attributi di estensione per gli oggetti utente possono essere utilizzati per l'emissione di attestazioni per le applicazioni. [L'uso degli attributi di estensione](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) dello schema di directory nelle attestazioni descrive come usare gli attributi di estensione dello schema di directory per inviare dati utente alle applicazioni nelle attestazioni di token.

Per altre informazioni sulle attestazioni di token, vedi:

- [Attestazioni nei token di accesso](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Attestazioni in un id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Attestazioni](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) previste nei token ID e nei token di accesso emessi da Azure AD B2C
- [Informazioni di riferimento sulle attestazioni del token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
