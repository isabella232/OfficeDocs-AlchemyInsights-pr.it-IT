---
title: Problemi dell'API di Microsoft Graph
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716199"
---
# <a name="microsoft-graph-api-issues"></a>Problemi dell'API di Microsoft Graph

Questo argomento può essere applicabile anche agli sviluppatori che usano ancora l'API Graph di Azure AD. È tuttavia consigliabile **utilizzare** Microsoft Graph per tutti gli scenari di gestione di directory, identità e accessi.

**Problemi di autenticazione o autorizzazione**

- Se l'app non è in grado di acquisire **token** per chiamare Microsoft Graph, seleziona La categoria Problema con il recupero di un token di accesso **(autenticazione)** di Microsoft Graph per ottenere assistenza e supporto più specifici in questo argomento.
- Se l'app riceve errori di autorizzazione **401 o 403** durante la chiamata a Microsoft Graph, seleziona la categoria Ottenere un errore di accesso negato **(autorizzazione)** dell'API di Microsoft Graph per ottenere assistenza e supporto più specifici in questo argomento.

**Si desidera utilizzare Microsoft Graph, ma non si è certi di dove iniziare**

- [Panoramica di Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Panoramica della gestione di identità e accessi in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Introduzione alla creazione di app di Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Testare le API di Microsoft Graph nel tenant o in un tenant demo

**Si vuole usare Microsoft Graph, ma supporta le API della directory v1.0 necessarie?**

Microsoft Graph è l'API consigliata per la gestione di directory, identità e accessi. Tuttavia, esistono ancora alcune lacune tra ciò che è possibile in Azure AD Graph e Microsoft Graph. Leggere gli articoli seguenti, in cui vengono evidenziate le differenze più aggiornate per agevolare la scelta:

- [Differenze tra i tipi di risorse tra Azure AD Graph e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Differenze di proprietà tra Azure AD Graph e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Differenze tra i metodi tra Azure AD e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**L'API che chiamo non funziona: dove posso eseguire altri test?**

**Microsoft Graph Explorer:** testa le API di Microsoft Graph nel tenant o in un tenant demo e controlla anche le query **di** esempio in Microsoft Graph Explorer.

**L'app è troppo lenta e viene anche limitato. Quali miglioramenti è possibile apportare?**

A seconda dello scenario, sono disponibili diverse opzioni per rendere l'applicazione più performante e, in alcuni casi, meno inclini a essere limitate dal servizio (quando si effettuano troppe chiamate).

- [Procedure consigliate per Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Invio in batch delle richieste](https://docs.microsoft.com/graph/json-batching)
- [Tenere traccia delle modifiche tramite query delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Ricevere notifiche delle modifiche tramite webhook](https://docs.microsoft.com/graph/webhooks)
- [Linee guida per la limitazione](https://docs.microsoft.com/graph/throttling)

**Dove è possibile trovare ulteriori informazioni su errori e problemi noti?**

- [Informazioni sulla risposta agli errori di Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Problemi noti di Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Dove è possibile verificare lo stato della disponibilità e della connettività del servizio?**

La disponibilità e la connettività dei servizi sottostanti a cui è possibile accedere tramite Microsoft Graph possono influire sulla disponibilità complessiva e sulle prestazioni di Microsoft Graph.

- Per l'integrità del servizio Azure Active Directory, controllare lo stato dei servizi sicurezza **e** identità elencati nella pagina [di stato di Azure.](https://azure.microsoft.com/status/)
- Per i servizi di Office che contribuiscono a Microsoft Graph, controllare lo stato dei servizi elencati nel dashboard sull'integrità [dei servizi di Office.](https://portal.office.com/adminportal/home#/servicehealth)

Gli errori di autorizzazione di Microsoft Graph possono essere il risultato di diversi problemi, la maggior parte dei quali genera un errore 401 o 403. Ad esempio, quanto segue può causare errori di autorizzazione:

- [Flussi di acquisizione di token di accesso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) non corretti
- [Ambiti di autorizzazione](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) non configurati correttamente
- Mancanza di [consenso](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Fine del supporto per Active Directory Authentication Library (ADAL) e l'API Graph di Azure AD (AAD Graph)_* _

_*A partire dal 30 giugno 2020**, non aggiungeremo più nuove funzionalità ad ADAL e Azure AD Graph. Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.

**A partire dal 30 giugno 2022,** microsoft terminerà il supporto per ADAL e Azure AD Graph e non fornirà più supporto tecnico o aggiornamenti della sicurezza.

Le app che usano ADAL nelle versioni esistenti del sistema operativo continueranno a funzionare dopo questo periodo, ma non riceveranno alcun supporto tecnico o aggiornamenti *della sicurezza.*

Le app che usano Azure AD Graph dopo questo periodo potrebbero non ricevere più risposte dall'endpoint di Azure AD Graph.

**Migrazione ADAL**

È consigliabile eseguire l'aggiornamento a [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), che include le funzionalità e gli aggiornamenti della sicurezza più recenti.

Se si usano app Microsoft, è importante sapere che Microsoft sta per eseguire la migrazione delle applicazioni a MSAL entro la scadenza del supporto, assicurandosi che trarranno vantaggio dai continui miglioramenti delle funzionalità e della sicurezza di MSAL.

1. [Consultare le domande frequenti su ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Informazioni su come eseguire la migrazione delle app in base alla piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Se ti serve aiuto per capire quale delle tue app usa ADAL, ti consigliamo di esaminare tutto il codice sorgente delle tue app e, se applicabile, contattare qualsiasi ISV o provider di app. Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.

**Migrazione Graph di AAD**

Per le applicazioni che usano Azure AD Graph, seguire le indicazioni per eseguire [la migrazione delle app Di Azure AD Graph a Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [L'elenco di controllo per la migrazione fornisce un punto di partenza](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Il portale di registrazione delle app Azure illustra quali applicazioni usano Graph di AAD. È consigliabile esaminare tutto il codice sorgente delle app e, se applicabile, contattare eventuali fornitori di software indipendenti o provider di app. Il supporto Tecnico Microsoft può anche fornire un elenco di tutti gli utilizzi di AAD Graph nel tenant.
3. Per consentire all'app di accedere ai dati in Microsoft Graph, l'utente o l'amministratore deve concedervi le autorizzazioni corrette tramite un processo di consenso. Nella [guida di riferimento alle autorizzazioni di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) sono elencate le autorizzazioni associate a ogni set principale di API di Microsoft Graph. Vengono inoltre fornite indicazioni su come utilizzare le autorizzazioni.
