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
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Utente singolo che non vede i componenti aggiuntivi in Outlook

È possibile che l'utente faccia parte di un ruolo che non dispone del parametro corretto di AppsForOfficeEnabled. Eseguire questo cmdlet per scoprire se il ruolo corretto è associato all'utente:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

Per ulteriori informazioni, vedere [Specificare gli amministratori e gli utenti in grado di installare e gestire componenti aggiuntivi per Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
