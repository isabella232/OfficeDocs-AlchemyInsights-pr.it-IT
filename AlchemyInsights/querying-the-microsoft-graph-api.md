---
title: Esecuzione di query sull'API di Microsoft Graph
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923243"
---
# <a name="querying-the-microsoft-graph-api"></a>Esecuzione di query sull'API di Microsoft Graph

Questo argomento può essere applicabile anche agli sviluppatori che usano ancora l'API Graph Azure AD. È tuttavia consigliabile **utilizzare** Microsoft Graph per tutti gli scenari di gestione di directory, identità e accessi.

**Problemi di autenticazione o autorizzazione**

- Se la tua app non è in grado di acquisire **token** per chiamare Microsoft Graph, seleziona Problema con il recupero di un token di accesso **(autenticazione)** categoria Microsoft Graph per ottenere assistenza e supporto più specifici su questo argomento.
- Se l'app riceve errori di autorizzazione **401 o 403** durante la chiamata a Microsoft Graph, seleziona la categoria Ottenere un errore di accesso negato **(autorizzazione)** API di Microsoft Graph per ottenere assistenza e supporto più specifici su questo argomento.

**Voglio usare Microsoft Graph, ma non so da dove iniziare**

Per ulteriori informazioni su Microsoft Graph, vedere:

- [Panoramica di Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Panoramica della gestione delle identità e degli accessi in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Introduzione alla creazione di app Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Testare le API di Microsoft Graph nel tenant o in un tenant demo

**Voglio usare Microsoft Graph, ma supporta le API della directory v1.0 necessarie?**

Microsoft Graph è l'API consigliata per la gestione di directory, identità e accessi. Tuttavia, esistono ancora alcune lacune tra ciò che è possibile in Azure AD Graph e Microsoft Graph. Leggere gli articoli seguenti, che evidenziano le differenze più aggiornate per agevolare la scelta:

- [Differenze tra i tipi di risorse tra Azure AD Graph e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Differenze di proprietà tra Azure AD Graph e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Differenze di metodo tra Azure AD e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Quando si esegue una query *sull'oggetto* utente, molte delle relative proprietà sono mancanti**

`GET https://graph.microsoft.com/v1.0/users`restituisce solo 11 proprietà, poiché Microsoft Graph automaticamente un set predefinito *di* proprietà utente da restituire. Se sono necessarie altre *proprietà utente,* utilizzare $select per selezionare le proprietà necessarie per l'applicazione. Provalo prima in **Microsoft Graph Explorer.**

**Alcuni valori delle proprietà utente *sono null* anche se sono impostati**

La spiegazione più probabile è che all'applicazione sia stata concessa *l'autorizzazione User.ReadBasic.All.* In questo modo l'applicazione può leggere un set limitato di proprietà utente, restituisce tutte le altre proprietà come null anche se sono state impostate in precedenza. Provare invece a concedere *all'applicazione l'autorizzazione User.Read.All.*

Per ulteriori informazioni, vedere [Microsoft Graph autorizzazioni utente.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**I'm having trouble using OData query parameters to filter data in my requests**

Sebbene Microsoft Graph supporti un'ampia gamma di parametri di query OData, molti di questi parametri non sono completamente supportati dai servizi directory (risorse che ereditano da *directoryObject*) in Microsoft Graph. Le stesse limitazioni presenti in Azure AD Graph persistono per la maggior parte in Microsoft Graph:

1. **Non supportato:**$count, $search e $filter valori *null* o *non Null*
2. **Non supportato:**$filter su determinate proprietà (vedere gli argomenti relativi alle risorse in cui è possibile filtrare le proprietà)
3. **Non supportato:** paging, filtro e ordinamento contemporaneamente
4. **Non supportato:** filtro in base a una relazione. Ad esempio, trovare tutti i membri del gruppo di progettazione che si trovano nel Regno Unito.
5. **Supporto parziale:**$orderby su *utente* (solo displayName e userPrincipalName) e *gruppo*
6. **Supporto** parziale: $filter (supporta solo il supporto *eq* *,* *startswith* *o*, e limited *any),*$expand (l'espansione delle relazioni di un singolo oggetto restituisce tutte le relazioni, ma l'espansione di un insieme di relazioni degli oggetti è limitata)

Per ulteriori informazioni, vedere [Personalizzare le risposte con i parametri di query.](https://docs.microsoft.com/graph/query-parameters)

**L'API che chiamo non funziona: dove posso eseguire altri test?**

**Microsoft Graph Explorer** - Testare le API di Microsoft Graph nel tenant o in un tenant demo e consultare anche le query di esempio **in** Microsoft Graph Explorer.

**Quando si esegue una query per i dati, sembra che si otterrà un set di dati incompleto**

Se si esegue una query su una raccolta , ad esempio gli utenti *,* Microsoft Graph utilizza i limiti delle pagine sul lato server in modo che i risultati siano sempre restituiti con dimensioni di pagina predefinite. L'app deve sempre prevedere di scorrere le raccolte restituite dal servizio.

Per altre informazioni, vedere:

- [Procedure consigliate Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging dei dati Graph Microsoft nella tua app](https://docs.microsoft.com/graph/paging)

**L'app è troppo lenta e viene anche limitato. Quali miglioramenti è possibile apportare?**

A seconda dello scenario, sono disponibili diverse opzioni per rendere l'applicazione più performante e, in alcuni casi, meno inclini a essere limitate dal servizio (quando si effettuano troppe chiamate).

Per altre informazioni, vedere:

- [Procedure consigliate Graph Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Invio in batch delle richieste](https://docs.microsoft.com/graph/json-batching)
- [Tenere traccia delle modifiche tramite query delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Ricevere notifiche delle modifiche tramite webhook](https://docs.microsoft.com/graph/webhooks)
- [Linee guida sulla limitazione](https://docs.microsoft.com/graph/throttling)

**Dove è possibile trovare ulteriori informazioni su errori e problemi noti?**

- [Informazioni sulla risposta Graph errore di Microsoft](https://docs.microsoft.com/graph/errors)
- [Problemi noti con Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Dove è possibile verificare lo stato della disponibilità e della connettività del servizio?**

La disponibilità e la connettività dei servizi sottostanti accessibili tramite Microsoft Graph possono influire sulla disponibilità e sulle prestazioni complessive di Microsoft Graph.

- Per Azure Active Directory integrità del servizio, controllare lo stato dei servizi di sicurezza **e** identità elencati nella pagina [stato di Azure.](https://azure.microsoft.com/status/)
- Per Office servizi che contribuiscono a Microsoft Graph, controllare lo stato dei servizi elencati nel dashboard Office [Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).
