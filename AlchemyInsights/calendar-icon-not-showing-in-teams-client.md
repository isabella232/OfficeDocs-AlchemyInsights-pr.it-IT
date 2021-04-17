---
title: L'icona del calendario non viene visualizzata nel client di Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819957"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="9198f-102">L'icona del calendario non viene visualizzata nel client di Teams</span><span class="sxs-lookup"><span data-stu-id="9198f-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="9198f-103">La scheda Calendario in Teams richiede l'accesso a una cassetta postale di Exchange tramite i Servizi Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9198f-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="9198f-104">La cassetta postale di Exchange può essere online o locale.</span><span class="sxs-lookup"><span data-stu-id="9198f-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="9198f-105">Per gli utenti online che non vedono la scheda Calendario, accertarsi che [abbiano la licenza per una cassetta postale di Exchange Online e che la cassetta postale sia abilitata](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="9198f-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="9198f-106">Se l'utente ha una cassetta postale valida in Exchange Online, ma non riesce ancora a visualizzare la scheda Calendario, può trattarsi di un problema di rete.</span><span class="sxs-lookup"><span data-stu-id="9198f-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="9198f-107">Usare l'[Analizzatore connettività remota Microsoft](https://testconnectivity.microsoft.com/) ed eseguire i **Test di connettività dei servizi Web di Microsoft Exchange** per l'utente interessato.</span><span class="sxs-lookup"><span data-stu-id="9198f-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="9198f-108">Infine, controllare in [App di Teams - Criteri di installazione app](https://admin.teams.microsoft.com/policies/app-setup) che l'app Calendario non sia stata rimossa dal criterio applicato all'utente (probabilmente il criterio **Globale** predefinito a livello di organizzazione).</span><span class="sxs-lookup"><span data-stu-id="9198f-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="9198f-109">Se gli utenti sono ospitati in locale, è necessario verificare che l'integrità della configurazione ibrida.</span><span class="sxs-lookup"><span data-stu-id="9198f-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="9198f-110">Usare la [Configurazione ibrida guidata](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) per la risoluzione dei problemi.</span><span class="sxs-lookup"><span data-stu-id="9198f-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="9198f-111">Si noti che [Teams richiede Exchange 2016 CU3 o versione successiva](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="9198f-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
