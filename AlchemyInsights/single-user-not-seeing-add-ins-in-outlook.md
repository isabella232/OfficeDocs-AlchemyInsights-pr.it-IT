---
title: Utente singolo che non vede i componenti aggiuntivi in Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719669"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="c0608-102">Utente singolo che non vede i componenti aggiuntivi in Outlook</span><span class="sxs-lookup"><span data-stu-id="c0608-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="c0608-103">È possibile che l'utente faccia parte di un ruolo che non dispone del parametro corretto di AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="c0608-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="c0608-104">Eseguire questo cmdlet per scoprire se il ruolo corretto è associato all'utente:</span><span class="sxs-lookup"><span data-stu-id="c0608-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="c0608-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="c0608-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="c0608-106">Per ulteriori informazioni, vedere [Specificare gli amministratori e gli utenti in grado di installare e gestire componenti aggiuntivi per Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="c0608-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
