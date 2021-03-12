---
title: Problemi relativi a una risorsa o a un'entità servizio
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/28/2021
ms.locfileid: "50716127"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemi relativi a una risorsa o a un'entità servizio

1. Se si è appena iniziato, gli oggetti applicazione e entità servizio [in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) descrivono la registrazione dell'applicazione, gli oggetti applicazione e le entità servizio in Azure Active Directory: cosa sono, come vengono usati e come sono correlati tra loro. Viene inoltre presentato uno scenario di esempio multi-tenant per illustrare la relazione tra l'oggetto applicazione di un'applicazione e gli oggetti entità servizio corrispondenti.
2. Per ulteriori informazioni sulla relazione tra applicazioni ed entità servizio, leggere le applicazioni e gli oggetti [entità servizio in Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [Procedura:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Usare il portale per creare un'applicazione Azure AD e un'entità servizio che possono accedere alle risorse illustra come creare una nuova applicazione Azure Active Directory (Azure AD) e un'entità servizio che possono essere usate con il controllo dell'accesso basato sui ruoli.
4. Con [l'API dell'entità](https://docs.microsoft.com/graph/api/resources/serviceprincipal)servizio, è possibile gestire a livello di programmazione le istanze delle applicazioni e controllare le attività che un'applicazione può eseguire all'interno del tenant.
5. [il tipo di risorsa servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) elenca tutte le proprietà e i metodi per il tipo di risorsa servicePrincipal.
6. [Le differenze tra i tipi di risorse tra Azure AD Graph e Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) evidenziano le differenze tra le risorse di Azure AD Graph e Microsoft Graph. Mostra le risorse con nomi diversi o che non sono disponibili. Vengono inoltre evidenziate le risorse disponibili nella versione beta di Microsoft Graph, ma non nella versione v1.0.

**Problemi con gli utenti guest**

- [Guida introduttiva:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Aggiungere utenti guest alla directory nel portale di Azure mostra come aggiungere un nuovo utente guest alla directory di Azure AD tramite il portale di Azure, inviare un invito e vedere l'aspetto del processo di riscatto degli inviti dell'utente guest.
- [Esercitazione: Creare flussi utente in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) mostra come creare alcuni flussi utente consigliati tramite il portale di Azure. Per informazioni su come configurare un flusso roPC (Resource Owner Password Credentials) nell'applicazione, vedere Configurare il flusso delle credenziali della password del proprietario della risorsa in Azure AD B2C.
