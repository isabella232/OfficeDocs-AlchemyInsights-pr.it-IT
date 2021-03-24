---
title: Problemi relativi al certificato o al segreto client di registrazione app
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
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123200"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="bf085-102">Problemi relativi al certificato o al segreto client di registrazione app</span><span class="sxs-lookup"><span data-stu-id="bf085-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="bf085-103">Il segreto client dell'applicazione scade?</span><span class="sxs-lookup"><span data-stu-id="bf085-103">Application client secret expiring?</span></span>

<span data-ttu-id="bf085-104">Indipendentemente dalla modalità di creazione dell'applicazione registrata, tramite il processo di registrazione standard nel portale di registrazione delle app o se l'entità servizio è stata creata nel tenant utilizzando il consenso dell'applicazione, sarà necessario creare un nuovo segreto client prima della scadenza di quella corrente e aggiornarne il codice dell'applicazione correlata.</span><span class="sxs-lookup"><span data-stu-id="bf085-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="bf085-105">Il periodo di validità massimo è 2 anni.</span><span class="sxs-lookup"><span data-stu-id="bf085-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="bf085-106">Come promemoria, il valore segreto deve essere registrato perché non sarà più visibile dopo aver lasciato la pagina Registrazioni app nel portale.</span><span class="sxs-lookup"><span data-stu-id="bf085-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="bf085-107">Per altre informazioni, vedi [Guida introduttiva: Registrare un'app nella](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) piattaforma di identità Microsoft e [Procedure consigliate per la piattaforma di identità Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="bf085-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="bf085-108">Per altre informazioni, vedi [Creare un'entità](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)servizio & app Azure AD nel portale - Piattaforma di identità Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bf085-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
