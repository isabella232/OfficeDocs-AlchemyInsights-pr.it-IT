---
title: Problemi relativi al consenso dell'amministratore
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 01/18/2021
ms.locfileid: "49888320"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="6fb29-102">Problemi relativi al consenso dell'amministratore</span><span class="sxs-lookup"><span data-stu-id="6fb29-102">Admin consent issues</span></span>

1. <span data-ttu-id="6fb29-103">Abilitare il [flusso di lavoro consenso](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) amministratore per consentire agli utenti di richiedere l'approvazione dell'amministratore direttamente dalla schermata di consenso.</span><span class="sxs-lookup"><span data-stu-id="6fb29-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="6fb29-104">Se l'utente o gli utenti dell'applicazione stanno visualizzando errori imprevisti durante il processo di consenso, vedere questo articolo per la risoluzione dei problemi: [errore imprevisto durante l'esecuzione del consenso a un'applicazione](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="6fb29-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="6fb29-105">Per ulteriori informazioni, vedere [consenso di amministratore sulla piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), modalità di funzionamento del [prompt di consenso](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) e come [valutare una richiesta di autorizzazione di amministratore a livello di tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="6fb29-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="6fb29-106">Le applicazioni che si integrano con Microsoft Identity Platform seguono un modello di autorizzazione che consente agli utenti e agli amministratori di controllare il modo in cui è possibile accedere ai dati.</span><span class="sxs-lookup"><span data-stu-id="6fb29-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="6fb29-107">L'implementazione del modello di autorizzazione è stata aggiornata sull'endpoint della piattaforma Microsoft Identity e modifica il modo in cui un'app deve interagire con la piattaforma Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="6fb29-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="6fb29-108">Per una panoramica di questo modello di autorizzazione, compresi gli ambiti, le autorizzazioni e il consenso, vedere [autorizzazioni e consenso nell'endpoint della piattaforma Microsoft Identity](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) .</span><span class="sxs-lookup"><span data-stu-id="6fb29-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>