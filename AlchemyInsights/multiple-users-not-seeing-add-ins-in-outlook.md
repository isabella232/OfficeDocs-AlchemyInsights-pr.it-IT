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
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Più utenti che non vedono i componenti aggiuntivi in Outlook

Se si eseguono i test dei componenti aggiuntivi di Outlook ma nessuno viene visualizzato, come primo passaggio di risoluzione dei problemi usare il cmdlet di PowerShell **Get-OrganizationConfig** per interrogare il parametro _AppsForOfficeEnabled_. Se la query restituisce un valore di **False**, impostare questo parametro su **True** usando il cmdlet **Set-OrganizationConfig**, in modo che i componenti aggiuntivi vengano visualizzati come previsto.

Si consiglia di evitare che il parametro _AppsForOfficeEnabled_ sia impostato su **False**. Il valore **False** sostituisce tutte le impostazioni dei ruoli Amministratore e Utente e impedisce che le nuove app vengano attivate da qualsiasi utente dell'organizzazione.

Per ulteriori informazioni, vedere [Specificare gli amministratori e gli utenti in grado di installare e gestire componenti aggiuntivi per Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).