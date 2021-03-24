---
title: Problemi relativi al proprietario della registrazione dell'app
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123195"
---
# <a name="app-registration-owner-issues"></a>Problemi relativi al proprietario della registrazione dell'app

Di seguito sono riportati i metodi disponibili per aggiungere entità come proprietari per le registrazioni delle app:

- Utilizzo del modulo di Azure AD PowerShell -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Riferimento: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Utilizzo dell'interfaccia della riga di comando di Azure - `az ad app owner add`

    Riferimento: [proprietario dell'app pubblicitaria az](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Utilizzo di MS Graph -

    Riferimento: [Aggiungere proprietario - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners

**Non è possibile visualizzare l'applicazione nel pannello Registrazioni app anche se si è proprietari di tale applicazione?**

Il proprietario di un'app non è un ruolo amministrativo. Se [l'impostazione Limita accesso al portale di amministrazione](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) di Azure AD è abilitata, solo l'amministratore potrà visualizzare le applicazioni nel portale di registrazione app. Per fare in modo che un proprietario possa visualizzare le applicazioni, disabilitare questa impostazione (impostare questa opzione su NO) o assegnare il ruolo di amministratore al proprietario solo per l'applicazione specifica. A questo scopo, tuttavia, sarà necessaria una licenza di Azure AD Premium P2 e si abiliterà [Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
