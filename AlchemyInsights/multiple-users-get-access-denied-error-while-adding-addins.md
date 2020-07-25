---
title: Più utenti ricevono un errore di accesso negato durante l'aggiunta di componenti aggiuntivi in Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397719"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Più utenti ricevono un errore di accesso negato durante l'aggiunta di componenti aggiuntivi in Outlook

È possibile specificare quali amministratori nell'organizzazione abbiano le autorizzazioni per installare e gestire i componenti aggiuntivi per Outlook. Inoltre è possibile specificare quali utenti nell'organizzazione abbiano le autorizzazioni per installare e gestire i componenti aggiuntivi per il proprio utilizzo.

Per dettagli, vedere [Specificare gli amministratori e gli utenti in grado di installare e gestire componenti aggiuntivi per Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Per verificare che siano state assegnate le autorizzazioni necessarie per un utente, sostituire <Role Name> con il nome del ruolo da verificare ed eseguire il comando seguente in PowerShell di Exchange Online:

Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers

In questo esempio viene mostrato come verificare a quale persona sono state assegnate le autorizzazioni per installare i componenti aggiuntivi dall'Office Store per l'organizzazione.

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

Nei risultati, Get-ManagementRoleAssignment, esaminare le voci nella colonna Utenti interessati.

Per informazioni dettagliate sulla sintassi e sui parametri, vedere [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 