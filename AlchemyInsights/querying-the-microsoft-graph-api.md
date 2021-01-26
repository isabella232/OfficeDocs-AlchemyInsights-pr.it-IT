---
title: Esecuzione di query nell'API di Microsoft Graph
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950715"
---
# <a name="querying-the-microsoft-graph-api"></a>Esecuzione di query nell'API di Microsoft Graph

Questo argomento potrebbe essere valido anche per gli sviluppatori che utilizzano ancora Azure AD Graph API. Tuttavia, **è consigliabile utilizzare** Microsoft Graph per tutti gli scenari di gestione delle directory, delle identità e degli accessi.

**Problemi di autenticazione o autorizzazione**

- Se l'app **non è in grado di acquisire token** per chiamare Microsoft Graph, scegli **un problema con la categoria ottenere un token di accesso (autenticazione)** di Microsoft Graph per ottenere assistenza e supporto più specifici su questo argomento.
- Se l'app **riceve gli errori di autorizzazione 401 o 403** quando si chiama Microsoft Graph, scegliere la categoria **ottenere un errore di accesso negato (autorizzazione)** Microsoft Graph API per ottenere assistenza e supporto più specifiche su questo argomento.

**Si desidera utilizzare Microsoft Graph, ma non si è certi da dove iniziare**

Per ulteriori informazioni su Microsoft Graph, vedere:

- [Panoramica di Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Panoramica della gestione delle identità e degli accessi in Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Guida introduttiva alla creazione di app di Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** -testare le API di Microsoft Graph nel tenant o un tenant demo

**Si desidera utilizzare Microsoft Graph, ma supporta le API della directory v 1.0 di cui ho bisogno?**

Microsoft Graph è l'API consigliata per la gestione delle directory, dell'identità e degli accessi. Tuttavia, vi sono ancora alcuni spazi vuoti tra ciò che è possibile fare in Azure AD Graph e Microsoft Graph. Esaminare gli articoli seguenti, in cui vengono evidenziate le differenze più aggiornate per facilitare la scelta:

- [Differenze tra i tipi di risorse tra Azure AD Graph e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Differenze tra le proprietà tra Azure AD Graph e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Differenze di metodo tra Azure AD e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Quando si esegue una query sull'oggetto *utente* , molte delle relative proprietà sono mancanti**

`GET https://graph.microsoft.com/v1.0/users` restituisce solo 11 proprietà, in quanto Microsoft Graph seleziona automaticamente un insieme predefinito di proprietà *utente* da restituire. Se sono necessarie altre proprietà *degli utenti* , utilizzare $Select per scegliere le proprietà necessarie per l'applicazione. Provare in **Microsoft Graph Explorer** per primo.

**Alcuni valori delle proprietà utente sono *null* anche se sono stati impostati**

La spiegazione più probabile è che all'applicazione sia stata concessa l'autorizzazione *User. ReadBasic. All* . In questo modo l'applicazione può leggere un insieme limitato di proprietà dell'utente, restituendo tutte le altre proprietà come null anche se sono stati precedentemente impostati. Provare a concedere invece l'autorizzazione *User. Read. All* dell'applicazione.

Per ulteriori informazioni, vedere [autorizzazioni utente di Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Si verificano problemi con i parametri di query OData per filtrare i dati nelle richieste personali**

Mentre Microsoft Graph supporta una vasta gamma di parametri di query OData, molti di questi parametri non sono completamente supportati dai servizi directory (risorse che ereditano da *directoryObject*) in Microsoft Graph. Le stesse limitazioni presenti in Azure AD Graph persistono per la maggior parte in Microsoft Graph:

1. **Non supportato**: $count, $search e $Filter su valori *null* o *non null*
2. **Non supportato**: $Filter su determinate proprietà (vedere Resource topics on quali proprietà sono filtrabili)
3. **Non supportato**: paging, filtro e ordinamento allo stesso tempo
4. **Non supportato**: filtro su una relazione. Ad esempio, trovare tutti i membri del gruppo di ingegneri che si trovano nel Regno Unito.
5. **Supporto parziale**: $OrderBy su *utente* (solo DisplayName e userPrincipalName) e *gruppo*
6. **Supporto parziale**: $Filter (supporta solo il supporto di *EQ*, *StartsWith* *o* *, e e limitate*), $Expand (l'espansione delle relazioni di un singolo oggetto restituisce tutte le relazioni, ma l'espansione di una raccolta di relazioni degli oggetti è *limitata)*

Per ulteriori informazioni, vedere [Customize Responses with query parameters](https://docs.microsoft.com/graph/query-parameters).

**L'API che chiamo non funziona-dove è possibile eseguire altre operazioni di testing?**

**Microsoft Graph Explorer** -testare le API di Microsoft Graph nel tenant o un tenant demo e consultare anche le **query di esempio** in Esplora risorse di Microsoft Graph.

**Quando si esegue una query per i dati, sembra che venga restituito un set di dati incompleto**

Se si esegue una query su un insieme (come *gli utenti*), Microsoft Graph utilizza limiti di pagina sul fianco del server in modo che i risultati vengano sempre restituiti con una dimensione di pagina predefinita. L'app dovrebbe sempre aspettarsi di passare alla pagina tramite gli insiemi restituiti dal servizio.

Per altre informazioni, vedere:

- [Procedure consigliate di Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging dei dati di Microsoft Graph nell'app](https://docs.microsoft.com/graph/paging)

**L'app è troppo lenta e viene anche strozzata. Quali miglioramenti è possibile apportare?**

A seconda dello scenario, sono disponibili diverse opzioni per rendere l'applicazione più performante e, in alcuni casi, meno incline a essere strozzata dal servizio (quando si effettuano troppe chiamate).

Per altre informazioni, vedere:

- [Procedure consigliate di Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Richieste di batch](https://docs.microsoft.com/graph/json-batching)
- [Registrare le modifiche tramite la query Delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Ricevere una notifica delle modifiche tramite webhook](https://docs.microsoft.com/graph/webhooks)
- [Linee guida per la limitazione](https://docs.microsoft.com/graph/throttling)

**Dove è possibile trovare ulteriori informazioni sugli errori e sui problemi noti?**

- [Informazioni sulla risposta di errore di Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Problemi noti relativi a Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Dove è possibile controllare lo stato della disponibilità e della connettività del servizio?**

La disponibilità del servizio e la connettività dei servizi sottostanti a cui è possibile accedere tramite Microsoft Graph possono influire sulla disponibilità complessiva e sulle prestazioni di Microsoft Graph.

- Per l'integrità dei servizi di Azure Active Directory, controllare lo stato di **Security + Identity** Services elencato nella [pagina di stato di Azure](https://azure.microsoft.com/status/).
- Per i servizi di Office che contribuiscono a Microsoft Graph, controllare lo stato dei servizi elencati nel [dashboard di integrità del servizio di Office](https://portal.office.com/adminportal/home#/servicehealth).
