---
title: Più utenti ricevono un errore di accesso negato durante l'aggiunta di componenti aggiuntivi in Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724367"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="79bcc-102">Più utenti ricevono un errore di accesso negato durante l'aggiunta di componenti aggiuntivi in Outlook</span><span class="sxs-lookup"><span data-stu-id="79bcc-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="79bcc-p101">È possibile specificare quali amministratori nell'organizzazione abbiano le autorizzazioni per installare e gestire i componenti aggiuntivi per Outlook. Inoltre è possibile specificare quali utenti nell'organizzazione abbiano le autorizzazioni per installare e gestire i componenti aggiuntivi per il proprio utilizzo.</span><span class="sxs-lookup"><span data-stu-id="79bcc-p101">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook. You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="79bcc-105">Per dettagli, vedere [Specificare gli amministratori e gli utenti in grado di installare e gestire componenti aggiuntivi per Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="79bcc-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="79bcc-106">Per verificare che siano state assegnate le autorizzazioni necessarie per un utente, sostituire <Role Name> con il nome del ruolo da verificare ed eseguire il comando seguente in PowerShell di Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="79bcc-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="79bcc-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="79bcc-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="79bcc-108">In questo esempio viene mostrato come verificare a quale persona sono state assegnate le autorizzazioni per installare i componenti aggiuntivi dall'Office Store per l'organizzazione.</span><span class="sxs-lookup"><span data-stu-id="79bcc-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="79bcc-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="79bcc-109">PowerShell</span></span>

<span data-ttu-id="79bcc-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="79bcc-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="79bcc-111">Nei risultati, Get-ManagementRoleAssignment, esaminare le voci nella colonna Utenti interessati.</span><span class="sxs-lookup"><span data-stu-id="79bcc-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="79bcc-112">Per informazioni dettagliate sulla sintassi e sui parametri, vedere [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="79bcc-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 