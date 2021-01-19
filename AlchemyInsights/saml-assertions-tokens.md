---
title: Asserzioni SAML (Tokens)
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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884590"
---
# <a name="saml-assertions-tokens"></a>Asserzioni SAML (Tokens)

1. I token SAML (Security Assertion Markup Language) sono rappresentazioni XML delle attestazioni. Per impostazione predefinita, i token SAML utilizzati da Windows Communication Foundation (WCF) negli scenari di sicurezza federata sono token emessi. Per ulteriori informazioni, vedere [token SAML e attestazioni](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. La piattaforma Microsoft Identity genera diversi tipi di token di sicurezza nell'elaborazione di ogni flusso di autenticazione. Il [riferimento alle attestazioni di token SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) descrive il formato, le caratteristiche di sicurezza e il contenuto dei token SAML 2,0.
3. Seguire le istruzioni riportate nelle [durata dei token configurabili in Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) per comprendere come configurare le durata del token.
4. Attenersi alla procedura descritta in [questo articolo](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) per informazioni su come configurare la crittografia dei token SAML di Azure ad.
5. In Azure AD, è possibile configurare le opzioni di firma del certificato e l'algoritmo di firma del certificato. Per ulteriori informazioni, vedere [Advanced Certificate Signing Options nel token SAML per le app di raccolta in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
