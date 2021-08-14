---
title: Ripristinare un gruppo Microsoft 365 eliminato
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959030"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Ripristinare un gruppo Microsoft 365 eliminato

È possibile ripristinare un gruppo Microsoft 365 o un Microsoft Teams eliminato entro 30 giorni dall'eliminazione.

1. Passare al [interfaccia di amministrazione di Microsoft 365](https://aka.ms/RestoreDeletedGroup) per accedere a un elenco dei gruppi e dei team eliminati.

    **Nota:** Accedere utilizzando l'account assegnato all'amministratore tenant o al ruolo di amministratore dei gruppi.

1. Selezionare il gruppo Microsoft 365/Teams da ripristinare e fare clic su **ripristina gruppo**.

    Se il gruppo non può essere ripristinato a causa di un indirizzo SMTP in conflitto, utilizzare il comando seguente per trovare l'oggetto che causa un conflitto e rimuovere l'indirizzo SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Nota:** In alcuni casi, il ripristino del gruppo e di tutti i relativi dati potrebbe richiedere fino a 24 ore.

    Per altre info o per informazioni su come ripristinare i gruppi tramite PowerShell, vedi Ripristinare un gruppo [Microsoft 365 eliminato.](https://go.microsoft.com/fwlink/?linkid=867802)