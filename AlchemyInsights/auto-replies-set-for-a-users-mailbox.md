---
title: 'Configurare le risposte automatiche per una cassetta postale '
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820938"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Configurare le risposte automatiche per la cassetta postale dell'utente

**Metodo 1**

1. Accedere al portale di Microsoft 365.

2. Passare a **Utenti > Utenti attivi** o **Gruppi > Cassette postali condivise** se è stata impostata questa opzione nella cassetta postale condivisa.

3. Selezionare un utente con una cassetta postale di Microsoft Exchange.

4. A destra, nel menu a comparsa passare a **Impostazioni di posta > Risposte automatiche**, se si tratta di una cassetta postale condivisa, basta fare clic su **Risposte automatiche** nel riquadro a comparsa.

**Metodo 2**

1. Accedere al portale di amministrazione di Microsoft 365 tramite le credenziali di amministratore.

2. Espandere **Interfacce di amministrazione**, poi fare clic su **Exchange**.

3. Fare clic sull'immagine nell'angolo in alto a destra, fare clic su **Altro utente** e poi selezionare la cassetta postale utente che si vuole modificare.

4. A sinistra, selezionare **Opzioni**, fare clic su **Organizza posta elettronica** e poi fare clic su **Risposte automatiche.**

**Metodo 3**

In PowerShell di Exchange Online, eseguire il cmdlet seguente:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Per altre informazioni sul cmdlet, vedere [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
