---
title: Problemi di accesso utente SSO senza problemi
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919203"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Problemi di accesso utente SSO senza problemi

Dopo l'autenticazione dell'utente, il browser memorizza nella cache le credenziali dell'utente, in modo che nello stesso browser l'applicazione eseguirà automaticamente l'accesso con lo stesso account. Ciò può rendere difficile per un altro utente o un singolo utente accedere a più account in un dispositivo. Per risolvere il problema: 1. Prova ad accedere in un altro browser. 2. Cancella la cache e/o i cookie del browser e riprova ad accedere.

Se si verificano ancora problemi di accesso, è consigliabile eseguire le operazioni seguenti per diagnosticare e automatizzare la procedura di risoluzione:

1. Installare [l'estensione del browser](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) sicuro app personali per aiutare Azure Active Directory (Azure AD) a fornire diagnosi e risoluzioni migliori quando si usa l'esperienza di test nel portale di Azure.
2. Riprodurre l'errore usando l'esperienza di test nella pagina di configurazione dell'app nel portale di Azure. Per ulteriori informazioni, vedere [Debug delle applicazioni Single #A0 basate su SAML.](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. Se si usa l'esperienza di test nel portale di Azure con l'estensione del browser sicuro app personali, è possibile **ignorare il passaggio 4.**
4. Per aprire la pagina di configurazione single #A0 basata su SAML:
    - Aprire il [portale di Azure](https://portal.azure.com/) e accedere come amministratore **globale** o **coadmin.**
    - Aprire **l'estensione di Azure Active Directory** selezionando Tutti **i** servizi nella parte superiore del menu di spostamento principale a sinistra.
    - Digitare "Azure Active Directory" nella casella di ricerca del filtro e selezionare **l'elemento di Azure Active Directory.**
    - Selezionare **Applicazioni aziendali** dal menu di spostamento sinistro di Azure Active Directory.
    - Selezionare **Tutte le applicazioni** per visualizzare un elenco di tutte le applicazioni. Se l'applicazione che si desidera visualizzare non  è visualizzata qui, utilizzare il controllo  Filtro nella parte superiore dell'elenco Tutte le applicazioni e impostare l'opzione Mostra su Tutte **le applicazioni.** 
    - Selezionare l'applicazione che si desidera configurare per l'accesso Single Sign-On.
    - Dopo il caricamento dell'applicazione, seleziona **Single #A0** dal menu di spostamento a sinistra dell'applicazione.
    - Selezionare **SSO basato su SAML.**
5. In base all'errore, per ulteriori informazioni sui passaggi consigliati da seguire, vedere Problemi di accesso alle app configurate per l'accesso [Single #A0 basato su SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. Per risolvere altri problemi di accesso utente, fare riferimento alle indicazioni seguenti:
    - [Protocollo SAML Sign-On singolo](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Procedura: Risolvere gli errori di accesso tramite i report di Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Richiesta di consenso imprevista](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Errore di consenso dell'utente](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problemi di accesso dalle app personali](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Errore nella pagina di accesso dell'applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problema durante l'accesso a un'app Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
