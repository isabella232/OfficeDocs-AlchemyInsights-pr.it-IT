---
title: Ripristinare un gruppo di Microsoft 365 eliminato
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645135"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="79125-102">Ripristinare un gruppo di Microsoft 365 eliminato</span><span class="sxs-lookup"><span data-stu-id="79125-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="79125-103">È possibile ripristinare un gruppo di Microsoft 365 o Microsoft Teams eliminato entro 30 giorni dall'eliminazione.</span><span class="sxs-lookup"><span data-stu-id="79125-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="79125-104">Accedere all'interfaccia di amministrazione di [Microsoft 365](https://aka.ms/RestoreDeletedGroup) per accedere a un elenco dei gruppi e dei team eliminati.</span><span class="sxs-lookup"><span data-stu-id="79125-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="79125-105">**Nota:** Accedere utilizzando l'account assegnato all'amministratore tenant o al ruolo di amministratore dei gruppi.</span><span class="sxs-lookup"><span data-stu-id="79125-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="79125-106">Selezionare il gruppo/Teams di Microsoft 365 eliminato da ripristinare e fare clic **su ripristina gruppo**.</span><span class="sxs-lookup"><span data-stu-id="79125-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="79125-107">Se il gruppo non può essere ripristinato a causa di un indirizzo SMTP in conflitto, utilizzare il comando seguente per trovare l'oggetto che causa un conflitto e rimuovere l'indirizzo SMTP:</span><span class="sxs-lookup"><span data-stu-id="79125-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="79125-108">**Nota:** In alcuni casi, il ripristino del gruppo e di tutti i relativi dati potrebbe richiedere fino a 24 ore.</span><span class="sxs-lookup"><span data-stu-id="79125-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="79125-109">Per altre info o per informazioni su come ripristinare i gruppi tramite PowerShell, vedi Ripristinare un gruppo [di Microsoft 365 eliminato.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="79125-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>