---
title: Ritardi nella ricezione di avvisi di SharePoint e OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771219"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="fe69a-102">Ritardi nella ricezione di avvisi di SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="fe69a-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="fe69a-103">Verificare innanzitutto la cartella posta indesiderata o posta indesiderata nella posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="fe69a-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="fe69a-104">Se **tutti gli avvisi provenienti da più file o raccolte sono ritardati**, visitare il [dashboard di integrità dei servizi](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) per verificare eventuali avvisi/incidenti che potrebbero verificarsi con SharePoint o Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe69a-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="fe69a-105">Il problema potrebbe essere relativo alla funzionalità di avviso di SharePoint o ai ritardi nei messaggi di posta elettronica tramite Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe69a-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="fe69a-106">Si noti inoltre se è in corso la recapito di altri messaggi di posta elettronica, altrimenti è probabile che si verifichino ritardi di Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe69a-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="fe69a-107">Se **un singolo avviso di un file o di una raccolta specifico non viene recapitato**, tentare di eliminarlo e ricrearlo.</span><span class="sxs-lookup"><span data-stu-id="fe69a-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="fe69a-108">Per ricreare l'avviso [, vedere gestire, visualizzare o eliminare gli avvisi di SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) .</span><span class="sxs-lookup"><span data-stu-id="fe69a-108">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="fe69a-109">Gli avvisi non possono essere inviati a un gruppo di distribuzione.</span><span class="sxs-lookup"><span data-stu-id="fe69a-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="fe69a-110">Sono supportati solo i gruppi di sicurezza e di O365.</span><span class="sxs-lookup"><span data-stu-id="fe69a-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="fe69a-111">Non è possibile personalizzare i modelli di posta elettronica di avviso.</span><span class="sxs-lookup"><span data-stu-id="fe69a-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="fe69a-112">Per ottenere tali operazioni, è necessario utilizzare il flusso di lavoro Microsoft Flow o SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="fe69a-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
