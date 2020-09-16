---
title: Ritardi nella ricezione di avvisi di SharePoint e OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727247"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="ed492-102">Ritardi nella ricezione di avvisi di SharePoint e OneDrive</span><span class="sxs-lookup"><span data-stu-id="ed492-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="ed492-103">Verificare innanzitutto la cartella posta indesiderata o posta indesiderata nella posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="ed492-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="ed492-104">Se **tutti gli avvisi provenienti da più file o raccolte sono ritardati**, visitare il [dashboard di integrità dei servizi](https://portal.office.com/adminportal/home?ref=/servicehealth) per verificare eventuali avvisi/incidenti che potrebbero verificarsi con SharePoint o Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed492-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="ed492-105">Il problema potrebbe essere relativo alla funzionalità di avviso di SharePoint o ai ritardi nei messaggi di posta elettronica tramite Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed492-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="ed492-106">Si noti inoltre se è in corso la recapito di altri messaggi di posta elettronica, altrimenti è probabile che si verifichino ritardi di Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed492-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="ed492-107">Se **un singolo avviso di un file o di una raccolta specifico non viene recapitato**, tentare di eliminarlo e ricrearlo.</span><span class="sxs-lookup"><span data-stu-id="ed492-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="ed492-108">Per ricreare l'avviso [, vedere gestire, visualizzare o eliminare gli avvisi di SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="ed492-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="ed492-109">Gli avvisi non possono essere inviati a un gruppo di distribuzione.</span><span class="sxs-lookup"><span data-stu-id="ed492-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="ed492-110">Sono supportati solo i gruppi di sicurezza e di O365.</span><span class="sxs-lookup"><span data-stu-id="ed492-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="ed492-111">Non è possibile personalizzare i modelli di posta elettronica di avviso.</span><span class="sxs-lookup"><span data-stu-id="ed492-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="ed492-112">Per ottenere tali operazioni, è necessario utilizzare il flusso di lavoro Microsoft Flow o SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="ed492-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
