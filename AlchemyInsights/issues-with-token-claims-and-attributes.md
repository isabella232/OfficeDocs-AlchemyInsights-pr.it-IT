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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029988"
---
# <a name="issues-with-token-claims-and-attributes"></a>Problemi relativi alle attestazioni e agli attributi dei token

**Update, Configure or Remove token Claims**

1. Utilizzando Azure Active Directory (Azure AD), è possibile [personalizzare il tipo di attestazione per l'attestazione di ruolo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) nel token di risposta visualizzato dopo l'autorizzazione di un'app.
2. Gli sviluppatori di applicazioni possono utilizzare attestazioni facoltative nelle applicazioni di Azure AD per specificare le attestazioni desiderate nei token inviati all'applicazione. Per ulteriori informazioni, vedere [fornire attestazioni facoltative per l'app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
3. [Configurare le attestazioni di gruppo per le applicazioni con Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Se si utilizza l'accesso Single Sign-on senza problemi nell'applicazione, vedere [Customize Claims issued nel token SAML for Enterprise Applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).

**Mapping degli attributi delle attestazioni**

1. Per configurare i criteri di mapping delle attestazioni tramite PowerShell, vedere [Customize Claims emitted in Tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
2. Gli attributi di estensione dello schema di directory consentono di archiviare dati aggiuntivi in Azure Active Directory per gli oggetti utente e altri oggetti directory, ad esempio gruppi, dettagli tenant, entità di servizio. Solo gli attributi di estensione per gli oggetti utente possono essere utilizzati per la creazione di attestazioni per le applicazioni. [Using Directory Schema Extension Attributes in Claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) descrive come utilizzare gli attributi di estensione dello schema di directory per l'invio dei dati degli utenti alle applicazioni in attestazioni di token.

Per ulteriori informazioni sulle attestazioni dei token, vedere:

- [Attestazioni nei token di accesso](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Attestazioni in un id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Attestazioni](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) che è possibile prevedere nei token di ID e nei token di accesso emessi da Azure ad B2C
- [Riferimento per le attestazioni di token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
