---
title: Dynamics 365-il dashboard errato viene visualizzato nell'interfaccia unificata di Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528555"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="789ba-102">Il dashboard errato viene visualizzato nell'interfaccia unificata di Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="789ba-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="789ba-103">Vi sono diversi motivi per cui è possibile che venga visualizzato un dashboard diverso da quello previsto:</span><span class="sxs-lookup"><span data-stu-id="789ba-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="789ba-104">L'utente ha impostato un dashboard predefinito dell'utente</span><span class="sxs-lookup"><span data-stu-id="789ba-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="789ba-105">In genere è possibile identificare un dashboard predefinito utente è impostato se il pulsante **Imposta come predefinito** non viene visualizzato nella barra dei comandi del dashboard.</span><span class="sxs-lookup"><span data-stu-id="789ba-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="789ba-106">Il dashboard predefinito dell'utente sostituirà tutti gli altri dashboard predefiniti, anche se il dashboard predefinito dell'utente non è incluso nell'app corrente.</span><span class="sxs-lookup"><span data-stu-id="789ba-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="789ba-107">Per annullare il dashboard predefinito, utilizzare la soluzione seguente.</span><span class="sxs-lookup"><span data-stu-id="789ba-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="789ba-108">Creare un nuovo dashboard personale.</span><span class="sxs-lookup"><span data-stu-id="789ba-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="789ba-109">Impostare il nuovo dashboard come predefinito dell'utente.</span><span class="sxs-lookup"><span data-stu-id="789ba-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="789ba-110">Eliminare il dashboard.</span><span class="sxs-lookup"><span data-stu-id="789ba-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="789ba-111">Il dashboard è impostato nella mappa del sito.</span><span class="sxs-lookup"><span data-stu-id="789ba-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="789ba-112">È possibile che sia stato impostato un dashboard predefinito dell'organizzazione selezionando un dashboard e scegliendo ' imposta come predefinito ' in ' Personalizza il sistema '.</span><span class="sxs-lookup"><span data-stu-id="789ba-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="789ba-113">Tuttavia, il dashboard definito nella Sitemap designer avrà la precedenza su questo dashboard, se l'utente può accedervi.</span><span class="sxs-lookup"><span data-stu-id="789ba-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="789ba-114">Per consentire agli utenti di visualizzare il dashboard impostato come predefinito dell'organizzazione, è possibile eseguire le operazioni seguenti:</span><span class="sxs-lookup"><span data-stu-id="789ba-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="789ba-115">Impostare il dashboard nella Sitemap</span><span class="sxs-lookup"><span data-stu-id="789ba-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="789ba-116">Rimuovere l'accesso al dashboard definito Sitemap per tali utenti</span><span class="sxs-lookup"><span data-stu-id="789ba-116">Remove access to the sitemap defined dashboard for those users</span></span>
