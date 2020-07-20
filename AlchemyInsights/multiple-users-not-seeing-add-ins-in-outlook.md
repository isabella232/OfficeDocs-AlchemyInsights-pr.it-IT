---
title: Più utenti che non vedono i componenti aggiuntivi in Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154581"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="69a9a-102">Più utenti che non vedono i componenti aggiuntivi in Outlook</span><span class="sxs-lookup"><span data-stu-id="69a9a-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="69a9a-103">Se si eseguono i test dei componenti aggiuntivi di Outlook ma nessuno viene visualizzato, come primo passaggio di risoluzione dei problemi usare il cmdlet di PowerShell **Get-OrganizationConfig** per interrogare il parametro _AppsForOfficeEnabled_.</span><span class="sxs-lookup"><span data-stu-id="69a9a-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="69a9a-104">Se la query restituisce un valore di **False**, impostare questo parametro su **True** usando il cmdlet **Set-OrganizationConfig**, in modo che i componenti aggiuntivi vengano visualizzati come previsto.</span><span class="sxs-lookup"><span data-stu-id="69a9a-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="69a9a-105">Si consiglia di evitare che il parametro _AppsForOfficeEnabled_ sia impostato su **False**.</span><span class="sxs-lookup"><span data-stu-id="69a9a-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="69a9a-106">Il valore **False** sostituisce tutte le impostazioni dei ruoli Amministratore e Utente e impedisce che le nuove app vengano attivate da qualsiasi utente dell'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="69a9a-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="69a9a-107">Per ulteriori informazioni, vedere [Specificare gli amministratori e gli utenti in grado di installare e gestire componenti aggiuntivi per Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="69a9a-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>