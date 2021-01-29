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
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/29/2021
ms.locfileid: "50043983"
---
# <a name="configure-and-customize-applications"></a>Configurare e personalizzare le applicazioni

**Configurare le applicazioni**

1. [Guida introduttiva: Configurare](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) le proprietà per un'applicazione nel tenant di Azure Active Directory (Azure AD) illustra come configurare alcune proprietà per un'app.
2. Per integrare le applicazioni con Azure Active Directory, è stata sviluppata una raccolta di [esercitazioni](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) che illustrano la configurazione.
3. [Come configurare un'applicazione proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) di applicazione consente di comprendere come configurare un'applicazione proxy di applicazione in Azure AD per esporre le applicazioni locali al cloud.
4. [Scaricare PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)e configurare l'applicazione: seguire le istruzioni in Configurare *PingAccess* per Azure AD per proteggere le applicazioni pubblicate tramite proxy di applicazione di Microsoft Azure AD nel sito Web Identità ping e scaricare la versione più recente di PingAccess.

**Errori di applicazione non configurata correttamente (AADSTS650056)**

1. Assicurati di accedere all'applicazione dall'indirizzo di accesso fornito dal proprietario dell'applicazione. In caso contrario, accedere all'applicazione tramite il normale processo. Nella maggior parte dei casi questa soluzione viene risolta automaticamente in modo naturale. In caso contrario, questo post può essere utile per la risoluzione dei problemi e la risoluzione dei problemi.
2. **Se l'organizzazione è proprietaria dell'applicazione** (ovvero la registrazione dell'applicazione è nell'organizzazione):
    - È consigliabile almeno aggiungere l'autorizzazione delegata `User.Read` `openid` da Microsoft **Graph.**
    - Verificare che l'applicazione e tutte le relative autorizzazioni siano autorizzate. Puoi verificarlo esaminando la colonna **Stato** della registrazione dell'applicazione in **Autorizzazioni API.**
    - In alcuni scenari, l'applicazione potrebbe essere di terze parti, ma potrebbe essere registrata nell'organizzazione. Verifica se questa applicazione è elencata nelle registrazioni delle app (non nelle applicazioni aziendali).
    - Se il messaggio di errore continua a essere visualizzato. Potrebbe quindi essere necessario creare l'URL di consenso descritto **nel passaggio 4.**
3. **Se l'organizzazione non è il proprietario dell'applicazione e la** utilizza come applicazione di terze parti:
    - Se sei l'amministratore globale/dell'azienda, dovrebbe essere visualizzata la schermata di consenso. Assicurati di selezionare la casella **"Consenso per conto dell'organizzazione".**
    - Se la schermata di consenso non è visualizzata, eliminare l'applicazione Enterprise e riprovare.
    - Se il messaggio di errore continua a essere visualizzato. Potrebbe quindi essere necessario creare l'URL di consenso descritto **nel passaggio 4.**
4. Compila manualmente **l'URL** di consenso da usare: se l'applicazione è progettata per accedere a una risorsa specifica, potresti non essere in grado di usare i pulsanti di consenso del portale di Azure, dovrai generare manualmente l'URL di consenso e usarlo.
    - Sarà necessario ottenere il e `{App-Id}` il `{App-Uri-Id}` dal proprietario dell'applicazione. `{Tenant-Id}` sarà l'identificatore del tenant. Questo sarà o `yourdomain.onmicrosoft.com` l'ID directory.
    - Se l'applicazione accede a se stessa per la risorsa, la proprietà `{App-Id}` e `{App-Uri-Id}` sarà la stessa.
5. Per ulteriori informazioni, vedere Problemi di accesso alle app configurate per [l'accesso Single #A0 basato su SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Personalizzare le applicazioni**

- Aggiungere la personalizzazione alla pagina di accesso di Azure Active Directory dell'organizzazione: usare il logo [dell'organizzazione](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) e le combinazioni di colori personalizzate per fornire un aspetto coerente alle pagine di accesso di Azure Active Directory (Azure AD).
- [Aggiungere il nome di dominio personalizzato usando il portale di Azure Active Directory:](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) ogni nuovo tenant di Azure AD viene fornito con un nome di dominio iniziale. Non è possibile modificare o eliminare il nome di dominio iniziale, ma è possibile aggiungere i nomi dell'organizzazione. L'aggiunta di nomi di dominio personalizzati consente di creare nomi utente familiari agli utenti.
