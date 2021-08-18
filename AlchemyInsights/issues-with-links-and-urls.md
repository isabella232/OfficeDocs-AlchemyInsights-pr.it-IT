---
title: Problemi relativi a collegamenti e URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321911"
---
# <a name="issues-with-links-and-urls"></a>Problemi relativi a collegamenti e URL

Gli URI di reindirizzamento o URL di risposta (le espressioni sono intercambiabili) sono gli URL usati da Microsoft Identity Platform per restituire i token richiesti dalle app. Per informazioni su questi URL, vedere gli articoli seguenti:

- [Flussi di autenticazione e scenari di applicazione](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios): informazioni sugli URI di reindirizzamento nella pagina **Registrazione app** per ogni scenario.
- [Limitazioni e restrizioni relative agli URI di reindirizzamento/URL di risposta](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Come registrare l'URI di reindirizzamento/URL di risposta appropriato per l'app**

Quando si accede con un’applicazione in fase di sviluppo e la finestra di dialogo per l’accesso restituisce il messaggio **AADSTS50011: L'URL di risposta specificato nella richiesta non corrisponde agli URL di risposta configurati per l'applicazione<your app ID>**, è necessario aggiungere alla registrazione dell'applicazione l'URI di reindirizzamento usato dal codice nella richiesta di token a Microsoft Identity Platform.

Per aggiungere un URL di risposta, passare alla scheda **Autenticazione** nella pagina di **registrazione dell'applicazione** nel portale di Azure e aggiungere una voce nella sezione **URI di reindirizzamento**. Il valore da immettere dipende dal tipo di applicazione che si sta sviluppando, come descritto di seguito:

- Per le applicazioni a pagina singola e le app Web, l'URL di risposta è un URL dell'applicazione. Vedere [Registrazione di una applicazione a pagina singola ](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) o [Registrazione di un'app Web usando il portale di Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Per le app desktop, il valore da scegliere dipende da:
    - La piattaforma (MacOS è diverso da Windows o Linux)
    - Il modo di acquisizione del token: in modo interattivo, con flusso di codice del dispositivo, con l'Autenticazione integrata di Windows [IWA] o con nome utente/password.
    Per informazioni dettagliate, vedere [App desktop - Registrazione delle app - URI di reindirizzamento](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Per le applicazioni per dispositivi mobili, l'URI di reindirizzamento dipende da:
    - La piattaforma (iOS/Android/UWP)
    - Le informazioni usate per creare l'app, ad esempio l'ID bundle in iOS e il nome del pacchetto e l'hash della firma in Android. La registrazione dell'app del portale di Azure è di aiuto. Per informazioni dettagliate, vedere [Configurazione della piattaforma e URI di reindirizzamento](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

**Nota**: le API Web e alcuni modi invisibili all'utente di acquisizione dei token (IWA e nome utente/password) non richiedono un URL di reindirizzamento.

**Se è stata distribuita un'applicazione Web e viene visualizzato un messaggio di mancata risposta dell'URL di risposta quando si testa l'app distribuita**

Aggiungere gli URI di reindirizzamento per tutte le posizioni in cui si sta distribuendo l'applicazione Web. Per altre informazioni, vedere [Registrazione di un'app Web tramite il portale di Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

**Nota**: aggiungere l'URI di reindirizzamento per una posizione immediatamente dopo la distribuzione dell'applicazione in tale posizione.

**Non è possibile registrare un numero sufficiente di URL di risposta**

Gli ISV hanno uno o più URI di reindirizzamento per ogni cliente. Si vuole eseguire la migrazione da ADAL/Azure AD v1.0 a MSAL/Microsoft Identity Platform e si è raggiunto il [numero massimo di URI di reindirizzamento](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Per risolvere il problema, [aggiungere gli URI di reindirizzamento ai servizi principali](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) che corrispondono a ciascun cliente.
