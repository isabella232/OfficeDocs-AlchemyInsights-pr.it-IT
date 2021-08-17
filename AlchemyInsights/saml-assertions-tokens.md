---
title: Asserzioni SAML (token)
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109244"
---
# <a name="saml-assertions-tokens"></a>Asserzioni SAML (token)

1. I token SAML (Security Assertions Markup Language) sono rappresentazioni XML delle attestazioni. Per impostazione predefinita, i token SAML Windows Communication Foundation (WCF) negli scenari di sicurezza federata vengono emessi token. Per ulteriori informazioni, vedere [Saml Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Il Microsoft Identity Platform genera diversi tipi di token di sicurezza nell'elaborazione di ogni flusso di autenticazione. [Il riferimento alle attestazioni di token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descrive il formato, le caratteristiche di sicurezza e il contenuto dei token SAML 2.0.
3. Segui le indicazioni in [Durata dei token configurabili in Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) informazioni su come configurare la durata dei token.
4. Seguire i passaggi descritti in [questo articolo](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) per informazioni su come configurare la crittografia token SAML di Azure AD.
5. In Azure AD, è possibile configurare le opzioni di firma dei certificati e l'algoritmo di firma del certificato. Per altre informazioni, vedi [Opzioni avanzate per la firma dei certificati nel token SAML per le](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)app della raccolta in Azure Active Directory .
