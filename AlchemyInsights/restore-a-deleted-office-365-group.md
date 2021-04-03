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
# <a name="restore-a-deleted-microsoft-365-group"></a>Ripristinare un gruppo di Microsoft 365 eliminato

È possibile ripristinare un gruppo di Microsoft 365 o Microsoft Teams eliminato entro 30 giorni dall'eliminazione.

1. Per accedere all'interfaccia di amministrazione di Microsoft 365 ed elencare i gruppi e i team eliminati, passare all'interfaccia di amministrazione di [Microsoft 365.](https://aka.ms/RestoreDeletedGroup)

    **Nota:** Accedere utilizzando l'account assegnato all'amministratore tenant o al ruolo di amministratore dei gruppi.

1. Selezionare il gruppo/Teams di Microsoft 365 eliminato da ripristinare e fare clic **su ripristina gruppo**.

    Se il gruppo non può essere ripristinato a causa di un indirizzo SMTP in conflitto, utilizzare il comando seguente per trovare l'oggetto che causa un conflitto e rimuovere l'indirizzo SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Nota:** In alcuni casi, il ripristino del gruppo e di tutti i relativi dati potrebbe richiedere fino a 24 ore.

    Per altre info o per informazioni su come ripristinare i gruppi tramite PowerShell, vedi Ripristinare un gruppo [di Microsoft 365 eliminato.](https://go.microsoft.com/fwlink/?linkid=867802)