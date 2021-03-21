---
title: Usare le raccolte di autenticazione
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897900"
---
# <a name="working-with-authentication-libraries"></a>Usare le raccolte di autenticazione

Per risolvere il problema della raccolta MSAL, esegui i seguenti passaggi raccomandati:

1. **Usare la raccolta MSAL**: [Raccolta di autenticazione della piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - Questo articolo illustra il supporto della raccolta di autenticazione di Microsoft per diversi tipi di applicazioni. Include collegamenti al codice sorgente della raccolta; descrive dove ottenere il pacchetto per il progetto dell'app, se la raccolta supporta l'autenticazione dell'utente, come accedere online alle API protette o entrambi.

2. **Risoluzione dei problemi di autenticazione**: la raccolta supporta numerosi flussi di autenticazione per l'uso in contesti applicativi differenti A seconda di come viene creata l'applicazione client, la raccolta MSAL può usare uno o più flussi di autenticazione supportati dalla piattaforma Microsoft Identity. Questi flussi possono produrre diversi tipi di token e codici di autorizzazione, e richiede l'uso di token differenti per farli funzionare.

3. **Token di accesso**: [token di accesso della piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Scopri come la tua API può convalidare e usare le attestazioni dei token di accesso. Tutta la documentazione di questo articolo, tranne quanto specificato, si applica solo ai token rilasciati per le API registrate. Non si applica ai token rilasciati per le API di proprietà di Microsoft, né può essere usata per convalidare il modo in cui la piattaforma Microsoft Identity emette i token per le API create dall'utente.

**Fine del supporto per Azure Active Directory Authentication Library (ADAL)**

- **A partire dal 30 giugno 2020,** non aggiungeremo altre funzionalità ad ADAL e Azure AD Graph. Microsoft continuerà a offrire supporto tecnico e aggiornamenti della sicurezza, ma non fornirà più aggiornamenti delle funzionalità.
- **A partire dal 30 giugno 2022,** Microsoft terminerà il supporto per ADAL e Graph di AAD e non fornirà più supporto tecnico o aggiornamenti della sicurezza.
- Le app che usano ADAL nelle versioni del sistema operativo esistenti continueranno a funzionare dopo tale data, ma non *riceveranno alcun supporto tecnico o aggiornamento di sicurezza*.
- Le app che usano Graph di Azure AD dopo tale data potrebbero non ricevere più risposte dall'endpoint Graph di Azure AD.

**Migrazione ADAL**

- Raccomandiamo di eseguire l'aggiornamento alla raccolta MSAL, che include le ultime funzionalità e gli aggiornamenti di sicurezza più recenti.
- Se usi Microsoft Apps, devi sapere che Microsoft sta completando la migrazione delle app su MSAL entro la data di scadenza del supporto, per assicurarsi che possano beneficiare dei miglioramenti continui della sicurezza e delle funzionalità di MSAL.

1. [Leggi le domande frequenti su ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Informazioni su come eseguire la migrazione delle app in base alla piattaforma](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Se hai ancora dubbi dopo aver letto la guida per la piattaforma della tua app, puoi scrivere un post su [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) con il tag [azure-ad-adal-deprecation] o aprire un ticket nell'archivio GitHub della raccolta. Vedi la sezione [Lingue e framework](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) dell'articolo **Paroramica su MSAL** per i collegamenti agli archivi di ciascuna raccolta.
4. **Se serve aiuto per capire quale app usa ADAL**, ti consigliamo di esaminare tutto il codice sorgente delle tue app. Se applicabile, contatta eventuali fornitori di software indipendenti (ISV) o provider di app. Il supporto Microsoft può fornire un elenco di tutte le app ADAL diverse da Microsoft nel tenant.







