---
title: Autorizzazioni API e processo di consenso
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
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379831"
---
# <a name="api-permissions-and-consent-process"></a>Autorizzazioni API e processo di consenso

Per consentire all'app di accedere ai dati in Microsoft Graph, l'utente o l'amministratore deve concedervi le autorizzazioni corrette tramite un processo di consenso. [Le informazioni di riferimento sulle](https://docs.microsoft.com/graph/permissions-reference) autorizzazioni di Microsoft Graph elencano le autorizzazioni associate a ogni set principale di API di Microsoft Graph. Vengono inoltre fornite indicazioni su come utilizzare le autorizzazioni.

**Configurare o aggiornare l'entità servizio**

- [Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) : in questo articolo viene illustrato come creare un nuovo oggetto servicePrincipal.
- Creare un'entità servizio & app Azure AD nel portale- Questo articolo illustra come creare una nuova applicazione Azure Active Directory (Azure AD) e [un'entità](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) servizio che può essere usata con il controllo di accesso basato sui ruoli.
- [App & entità](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) servizio in Azure AD - Questo articolo descrive la registrazione dell'applicazione, gli oggetti applicazione e le entità servizio in Azure Active Directory: cosa sono, come vengono usate e come sono correlate tra loro.

**Aggiungere o aggiornare la registrazione dell'app e fornire il consenso dell'amministratore**

- [Creare una registrazione dell'app:](https://docs.microsoft.com/graph/api/application-post-applications) questo articolo illustra come creare un nuovo oggetto applicazione.
- [Aggiornare la registrazione di un'app - Autorizzazioni API-](https://docs.microsoft.com/graph/api/application-update) Questo articolo illustra come aggiornare le proprietà di un oggetto applicazione.
- [Fornire il consenso dell'amministratore](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - Per il consenso e il consenso dell'amministratore in generale, è necessario che un amministratore concedi esplicitamente il consenso.
- [RBAC (beta):](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) contenitore di gestione dei ruoli per le definizioni di ruolo unificate e le assegnazioni di ruolo per i provider RBAC di Microsoft 365 che supportano più entità e più ambiti in una singola assegnazione di ruolo. È diverso dal *tipo di risorsa rbacApplication.* Microsoft Intune è un esempio di tale provider RBAC. Un'assegnazione di ruolo in Intune può avere una matrice di entità e una matrice di gruppi di ambiti. **Si tratta di una versione beta, ovvero è ancora in fase di sviluppo e non è consigliata per l'utilizzo in produzione.**
