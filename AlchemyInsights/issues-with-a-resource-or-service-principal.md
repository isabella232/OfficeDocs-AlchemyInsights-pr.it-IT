---
title: Problemi con una risorsa o un'entità servizio
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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028080"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problemi con una risorsa o un'entità servizio

1. Se si è appena iniziato, gli oggetti application e entità servizio [in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) descrivono la registrazione dell'applicazione, gli oggetti applicazione e le entità servizio in Azure Active Directory: cosa sono, come vengono usati e come sono correlati tra loro. Viene inoltre presentato uno scenario di esempio multi-tenant per illustrare la relazione tra l'oggetto applicazione di un'applicazione e gli oggetti entità servizio corrispondenti.
2. Per ulteriori informazioni sulla relazione tra applicazioni ed entità servizio, leggere applicazioni e oggetti entità [servizio in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Procedura:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Usare il portale per creare un'applicazione Azure AD e un'entità servizio che possono accedere alle risorse illustra come creare una nuova applicazione di Azure Active Directory (Azure AD) e un'entità servizio che possono essere usate con il controllo di accesso basato sui ruoli.
4. Con [l'API dell'entità](https://docs.microsoft.com/graph/api/resources/serviceprincipal)servizio è possibile gestire a livello di programmazione le istanze delle applicazioni e controllare le attività che un'applicazione può eseguire all'interno del tenant.
5. [servicePrincipal elenca tutte](https://docs.microsoft.com/graph/api/resources/serviceprincipal) le proprietà e i metodi per il tipo di risorsa servicePrincipal.
6. [Le differenze tra i tipi](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) di risorse tra Azure AD Graph e Microsoft Graph evidenziano le differenze tra Azure AD Graph e le risorse Graph Microsoft. Mostra le risorse con nomi diversi o che non sono disponibili. vengono inoltre evidenziate le risorse disponibili nella versione beta di Microsoft Graph ma non nella versione v1.0.

**Problemi con gli utenti guest**

- [Guida introduttiva:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Add guest users to your directory in the Azure portal shows you how to add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.
- [Tutorial: Create user flows in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) shows you how to create some recommended user flows by using the Azure portal. Per informazioni su come configurare un flusso roPC (Resource Owner Password Credentials) nell'applicazione, vedere Configure the resource owner password credentials flow in Azure AD B2C.
