---
title: L'icona del calendario non viene visualizzata nel client Microsoft Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576519"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="309d2-102">L'icona del calendario non viene visualizzata nel client Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="309d2-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="309d2-103">La scheda **Calendario** in teams richiede l'accesso a una cassetta postale di Exchange tramite i servizi Web di Exchange.</span><span class="sxs-lookup"><span data-stu-id="309d2-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="309d2-104">La cassetta postale di Exchange può essere online o locale.</span><span class="sxs-lookup"><span data-stu-id="309d2-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="309d2-105">Per gli utenti online che non vedono la scheda **Calendario** , accertarsi che [siano concessi in licenza per una cassetta postale di Exchange Online e che la cassetta postale sia abilitata](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="309d2-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="309d2-106">Se gli utenti sono ospitati in locale, è necessario verificare che la configurazione ibrida sia integra.</span><span class="sxs-lookup"><span data-stu-id="309d2-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="309d2-107">Usare la [Configurazione ibrida guidata](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) per la risoluzione dei problemi.</span><span class="sxs-lookup"><span data-stu-id="309d2-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="309d2-108">Si noti che [Teams richiede Exchange 2016 CU3 o versione successiva](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="309d2-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="309d2-109">Per ulteriori informazioni e procedure per la risoluzione dei problemi, vedere risolvere i problemi relativi all' [interazione di Microsoft teams e Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="309d2-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
