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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597447"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Ripristinare un gruppo di Microsoft 365 eliminato

È possibile ripristinare un gruppo di Microsoft 365 o Microsoft Teams eliminato entro 30 giorni dall'eliminazione.

1. Accedere all'interfaccia di amministrazione di [Microsoft 365](https://aka.ms/RestoreDeletedGroup) per accedere ed elencare i gruppi e i team eliminati.

    **Nota:** Accedere utilizzando l'account assegnato all'amministratore tenant o al ruolo di amministratore dei gruppi.

1. Selezionare il gruppo/Teams di Microsoft 365 eliminato da ripristinare e fare clic **su ripristina gruppo**.

    Se il gruppo non può essere ripristinato a causa di un indirizzo SMTP in conflitto, utilizzare il comando seguente per trovare l'oggetto che causa un conflitto e rimuovere l'indirizzo SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Nota:** In alcuni casi, il ripristino del gruppo e di tutti i relativi dati potrebbe richiedere fino a 24 ore.

    Per altre info o per informazioni su come ripristinare i gruppi tramite PowerShell, vedi Ripristinare un gruppo [di Microsoft 365 eliminato.](https://go.microsoft.com/fwlink/?linkid=867802)