---
title: Gestione delle impostazioni esterne
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 02/17/2021
ms.locfileid: "50282835"
---
# <a name="managing-external-settings"></a><span data-ttu-id="8a894-102">Gestione delle impostazioni esterne</span><span class="sxs-lookup"><span data-stu-id="8a894-102">Managing External Settings</span></span>

<span data-ttu-id="8a894-103">**Annuncio**</span><span class="sxs-lookup"><span data-stu-id="8a894-103">**Announcement**</span></span>

- <span data-ttu-id="8a894-104">[Deprecazione del supporto per l'accesso WebView da parte di Google a partire dal 4 gennaio 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="8a894-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="8a894-105">Controllare se le proprie app sono interessate seguendo le indicazioni di Google sulla verifica della compatibilità</span><span class="sxs-lookup"><span data-stu-id="8a894-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="8a894-106">Assicurarsi di usare la Webview di sistema o il browser di sistema durante l'accesso degli utenti con account consumer Google.</span><span class="sxs-lookup"><span data-stu-id="8a894-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="8a894-107">**Gestire le impostazioni per gli inviti**</span><span class="sxs-lookup"><span data-stu-id="8a894-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="8a894-108">Verificare di avere configurato le [impostazioni per la collaborazione esterna](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) in modo da consentire di inviare inviti alle persone appropriate.</span><span class="sxs-lookup"><span data-stu-id="8a894-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="8a894-109">**Gestire le autorizzazioni relative all'accesso degli utenti guest**</span><span class="sxs-lookup"><span data-stu-id="8a894-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="8a894-110">Gli amministratori globali possono gestire le autorizzazioni relative all'accesso guest nella directory tramite il portale di Azure, configurandole nella pagina Impostazioni di collaborazione esterna.</span><span class="sxs-lookup"><span data-stu-id="8a894-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="8a894-111">[Altre informazioni su questa impostazione](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="8a894-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="8a894-112">Se si vuole che gli utenti guest possano accedere ad app come Teams o SharePoint, verificare di averle configurate in modo da consentire l'accesso guest.</span><span class="sxs-lookup"><span data-stu-id="8a894-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="8a894-113">Altre informazioni sulle [Impostazioni di Teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) e [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="8a894-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="8a894-114">**Configurazione degli inviti:**</span><span class="sxs-lookup"><span data-stu-id="8a894-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="8a894-115">Abilitare la collaborazione esterna B2B e gestire gli utenti che possono invitare guest</span><span class="sxs-lookup"><span data-stu-id="8a894-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8a894-116">Consentire o bloccare gli inviti a utenti di specifiche organizzazioni</span><span class="sxs-lookup"><span data-stu-id="8a894-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="8a894-117">**Configurazione dei provider di identità consentiti:**</span><span class="sxs-lookup"><span data-stu-id="8a894-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="8a894-118">Federazione di Google</span><span class="sxs-lookup"><span data-stu-id="8a894-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8a894-119">Federazione diretta</span><span class="sxs-lookup"><span data-stu-id="8a894-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8a894-120">Autenticazione con passcode monouso tramite indirizzo di posta elettronica</span><span class="sxs-lookup"><span data-stu-id="8a894-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
