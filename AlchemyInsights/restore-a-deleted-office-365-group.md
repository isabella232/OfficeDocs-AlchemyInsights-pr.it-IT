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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505690"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="b06a5-102">Ripristinare un gruppo di Microsoft 365 eliminato</span><span class="sxs-lookup"><span data-stu-id="b06a5-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="b06a5-103">È possibile ripristinare un gruppo di Microsoft 365 o Microsoft Teams eliminato entro 30 giorni dall'eliminazione.</span><span class="sxs-lookup"><span data-stu-id="b06a5-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="b06a5-104">Per accedere all'interfaccia di amministrazione di Microsoft 365 ed elencare i gruppi e i team eliminati, passare all'interfaccia di amministrazione di [Microsoft 365.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="b06a5-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="b06a5-105">**Nota:** Accedere utilizzando l'account assegnato all'amministratore tenant o al ruolo di amministratore dei gruppi.</span><span class="sxs-lookup"><span data-stu-id="b06a5-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="b06a5-106">Selezionare il gruppo/Teams di Microsoft 365 eliminato da ripristinare e fare clic **su ripristina gruppo**.</span><span class="sxs-lookup"><span data-stu-id="b06a5-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="b06a5-107">Se il gruppo non può essere ripristinato a causa di un indirizzo SMTP in conflitto, utilizzare il comando seguente per trovare l'oggetto che causa un conflitto e rimuovere l'indirizzo SMTP:</span><span class="sxs-lookup"><span data-stu-id="b06a5-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="b06a5-108">**Nota:** In alcuni casi, il ripristino del gruppo e di tutti i relativi dati potrebbe richiedere fino a 24 ore.</span><span class="sxs-lookup"><span data-stu-id="b06a5-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="b06a5-109">Per altre info o per informazioni su come ripristinare i gruppi tramite PowerShell, vedi Ripristinare un gruppo [di Microsoft 365 eliminato.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="b06a5-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>