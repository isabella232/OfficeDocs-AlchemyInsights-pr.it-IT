---
title: Più oggetti hanno lo stesso indirizzo di posta elettronica come identità
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724619"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Più oggetti hanno lo stesso indirizzo di posta elettronica come identità

**Più oggetti**

Una delle cause più comuni di questo errore consiste nell’impossibilità di instradare correttamente una richiesta di Outlook Web App in presenza di più oggetti con lo stesso indirizzo di posta elettronica come identità. Per trovare tali oggetti, eseguire i comandi seguenti:

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

Per risolvere il problema, rimuovere gli oggetti con la stessa identità di posta elettronica e verificare che sia presente un singolo oggetto con una identità di posta elettronica specifica e che il relativo tipo di destinatario sia UserMailbox.

**Lo stesso indirizzo viene usato per le cassette postali aziendali e degli utenti privati**

Un’altra causa consiste nell’usare lo stesso indirizzo per le cassette postali aziendali e degli utenti privati. In questo caso, è necessario che l'utente modifichi il suo alias consumer principale finché Cafe non supporta questo scenario. Si tratta di un errore permanente che non scompare senza un intervento.

Per informazioni dettagliate, vedere [Cambiare l'indirizzo di posta elettronica o il numero di telefono per l’account Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).