---
title: Configurare SSO (Seamless Single Sign-On)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966041"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Configurare SSO (Seamless Single Sign-On)

**Configurare le applicazioni**

1. È consigliabile ottenere i valori dal fornitore dell'applicazione. È possibile immettere manualmente i valori o caricare un file di metadati per estrarre il valore dei campi.
2. Molte app sono già state preconfigurato per l'utilizzo con Azure AD. Queste app sono elencate nella raccolta di app che è possibile esplorare quando si aggiunge un'app al tenant di Azure AD. La [serie introduttiva](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) illustra il processo.
3. Per creare un'applicazione non di raccolta, puoi fare clic su **+ Crea** il tuo pulsante Applicazione e assegnare un nome all'applicazione.
    - Per impostazione predefinita, seleziona Integra qualsiasi altra applicazione non presente nella raccolta, che è **l'opzione** corretta per le applicazioni non della raccolta.
    - Dopo aver fatto **clic su Crea** dopo aver specificato il nome per l'applicazione, verrà creata una nuova applicazione non Enterprise raccolta.
    - È quindi possibile passare a **Single Sign-on** in **Gestisci** dell'applicazione e sarà possibile visualizzare tecniche diverse per l'implementazione nell'ambiente.

**Configurare SSO semplice per un'applicazione specifica**

Per le app nella raccolta troverai istruzioni dettagliate e dettagliate. Per accedere ai passaggi, puoi sfogliare un elenco di tutte le esercitazioni di configurazione delle app in Esercitazioni sulla [configurazione dell'app SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Configurare il servizio SSO basato su SAML**

1. [Guida introduttiva: Configurare SSO (Single Sign-On)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)basato su SAML per un'applicazione nel tenant di Azure Active Directory (Azure AD).
2. Per ulteriori informazioni sull'opzione basata su SAML per single sign-on, vedere [Understand SAML-based single sign-on.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Per informazioni sulle richieste e le risposte di autenticazione SAML 2.0 supportate da Azure Active Directory (Azure AD) per Single Sign-On (SSO), vedere [Single Sign-On SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Per informazioni su come creare e configurare un single sign-on basato su SAML (SSO) per l'applicazione in Azure Active Directory (Azure AD) usando l'API Microsoft Graph, vedere [Configure SAML-based Single Sign-On for your application using the Microsoft Graph API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Per informazioni su come Azure AD usa il protocollo SAML, [vedi Come il Microsoft Identity Platform usa il protocollo SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Configurare token e attestazioni**

1. [Procedura: personalizzare le attestazioni emesse nel token SAML per le applicazioni aziendali.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Per informazioni su come configurare le attestazioni tramite PowerShell, vedere Procedura: Personalizzare le attestazioni emesse nei token per [un'app specifica in un tenant (anteprima).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Per informazioni su come configurare attestazioni facoltative, vedi [Procedura: Fornire attestazioni facoltative per la tua app.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Per informazioni su come usare gli attributi dell'estensione dello schema di directory per l'invio di dati utente alle applicazioni nelle attestazioni di token, vedere [Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Per informazioni su come configurare la durata dei token, vedi Durata dei token configurabili nel Microsoft Identity Platform [(anteprima).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Configurare i criteri di durata dei token (anteprima):](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) in questo articolo viene descritto uno scenario di criteri comuni che consente di imporre nuove regole per la durata dei token. Nell'esempio viene illustrato come creare un criterio che richiede agli utenti di eseguire l'autenticazione con maggiore frequenza nella tua app Web.

**Risolvere i problemi di configurazione SSO**

- Per le domande frequenti su Azure Active Directory single Sign-On (SSO senza soluzione di continuità), vedere Azure Active Directory [Accesso Single Sign-On senza](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)soluzione di continuità: domande frequenti .
- Per informazioni sulla risoluzione dei problemi comuni relativi a Azure Active Directory (Azure AD) Seamless Single Sign-On (SSO senza soluzione di continuità), vedere [Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
