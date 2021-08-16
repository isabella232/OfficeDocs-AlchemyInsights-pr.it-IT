---
title: Configurare e personalizzare le applicazioni
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
- "9004334"
- "7733"
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044992"
---
# <a name="configure-and-customize-applications"></a>Configurare e personalizzare le applicazioni

**Configurare le applicazioni**

1. [Guida introduttiva: Configure properties for an application in your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) mostra come configurare alcune delle proprietà per un'app.
2. Per integrare le applicazioni con Azure Active Directory, è stata sviluppata una raccolta di [esercitazioni](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) che illustrano la configurazione.
3. [Come configurare un'applicazione proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) di applicazione consente di comprendere come configurare un'applicazione proxy di applicazione in Azure AD per esporre le applicazioni locali al cloud.
4. [Scaricare PingAccess e](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)configurare l'applicazione: seguire le istruzioni in *Configurare PingAccess* per Azure AD per proteggere le applicazioni pubblicate tramite proxy di applicazione Microsoft Azure AD nel sito Web Identità ping e scaricare la versione più recente di PingAccess.

**Errori dell'applicazione non configurata (AADSTS650056)**

1. Assicurati di accedere all'applicazione dall'indirizzo di accesso fornito dal proprietario dell'applicazione. In caso contrario, accedere all'applicazione tramite il processo normale. Nella maggior parte dei casi questa soluzione viene risolta automaticamente in modo naturale. In caso contrario, questo post può essere utile per risolvere i problemi e risolverli.
2. **Se l'organizzazione è proprietaria dell'applicazione** (ovvero la registrazione dell'applicazione è nell'organizzazione):
    - Come minimo, è consigliabile aggiungere l'autorizzazione o delegata `User.Read` `openid` da Microsoft **Graph.**
    - Verificare che l'applicazione e tutte le relative autorizzazioni siano autorizzate. Puoi verificarlo esaminando la colonna **Stato** della registrazione dell'applicazione in **Autorizzazioni API.**
    - In alcuni scenari, l'applicazione potrebbe essere di terze parti, ma potrebbe essere registrata nell'organizzazione. Verifica se questa applicazione è elencata nelle registrazioni dell'app (non Enterprise applicazioni).
    - Se si continua a visualizzare questo messaggio di errore. Potrebbe quindi essere necessario creare l'URL di consenso descritto **nel passaggio 4.**
3. **Se l'organizzazione non è il proprietario dell'applicazione e la utilizza come** applicazione di terze parti:
    - Se sei l'amministratore globale/aziendale, dovrebbe essere visualizzata la schermata di consenso. Assicurati di selezionare la casella **"Consenso per conto dell'organizzazione".**
    - Se non viene visualizzata la schermata di consenso, eliminare l'Enterprise e riprovare.
    - Se si continua a visualizzare questo messaggio di errore. Potrebbe quindi essere necessario creare l'URL di consenso descritto **nel passaggio 4.**
4. **Creare manualmente l'URL** di consenso da usare: se l'applicazione è progettata per accedere a una risorsa specifica, potrebbe non essere possibile usare i pulsanti di consenso dal portale di Azure, sarà necessario generare manualmente l'URL di consenso e usarlo.
    - Sarà necessario ottenere il e `{App-Id}` `{App-Uri-Id}` dal proprietario dell'applicazione. `{Tenant-Id}` sarà l'identificatore del tenant. Questo sarà o `yourdomain.onmicrosoft.com` l'ID directory.
    - Se l'applicazione accede a se stessa per la risorsa, il `{App-Id}` e `{App-Uri-Id}` sarà lo stesso.
5. Per altre informazioni, vedi Problemi di accesso alle app configurate per [il single sign-on basato](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)su SAML.

**Personalizzare le applicazioni**

- Aggiungere la personalizzazione alla pagina di accesso Azure Active Directory [dell'organizzazione-](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) Usare il logo dell'organizzazione e le combinazioni di colori personalizzate per offrire un aspetto coerente alle pagine di accesso di Azure Active Directory (Azure AD).
- [Aggiungi il nome di dominio personalizzato usando il portale Azure Active Directory-](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) Ogni nuovo tenant di Azure AD viene fornito con un nome di dominio iniziale. Non è possibile modificare o eliminare il nome di dominio iniziale, ma è possibile aggiungere i nomi dell'organizzazione. L'aggiunta di nomi di dominio personalizzati consente di creare nomi utente familiari agli utenti.
