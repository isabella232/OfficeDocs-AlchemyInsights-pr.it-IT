---
title: Autorizzazioni e autorizzazione API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951895"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="47083-102">Autorizzazioni e autorizzazione API</span><span class="sxs-lookup"><span data-stu-id="47083-102">API permissions and consent</span></span>

<span data-ttu-id="47083-103">Le applicazioni che si integrano con Microsoft Identity Platform seguono un modello di autorizzazione che consente agli utenti e agli amministratori di controllare il modo in cui è possibile accedere ai dati.</span><span class="sxs-lookup"><span data-stu-id="47083-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="47083-104">L'implementazione del modello di autorizzazione è stata aggiornata sull'endpoint della piattaforma Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="47083-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="47083-105">Viene modificato il modo in cui un'app deve interagire con la piattaforma Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="47083-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="47083-106">Le [autorizzazioni e il consenso nell'endpoint della piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) riguardano i concetti di base di questo modello di autorizzazione, compresi gli ambiti, le autorizzazioni e il consenso.</span><span class="sxs-lookup"><span data-stu-id="47083-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="47083-107">Il [Framework di consenso di Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) semplifica lo sviluppo di applicazioni Web multi-tenant e native client.</span><span class="sxs-lookup"><span data-stu-id="47083-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="47083-108">Queste applicazioni consentono l'accesso da parte degli account utente da un tenant di Azure AD diverso da quello in cui è registrata l'applicazione.</span><span class="sxs-lookup"><span data-stu-id="47083-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="47083-109">Potrebbe anche essere necessario accedere alle API Web, ad esempio l'API di Microsoft Graph (per accedere a Azure AD, Intune e servizi in Microsoft 365) e altre API dei servizi Microsoft, oltre alle proprie API Web.</span><span class="sxs-lookup"><span data-stu-id="47083-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

