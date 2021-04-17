---
title: Accedere a Windows 10 senza usare una password
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830550"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Accedere a Windows 10 senza usare una password

Per evitare di dover digitare una password all'avvio di Windows, ti consigliamo di usare una delle opzioni di accesso sicuro di Windows Hello, ad esempio un PIN, un riconoscimento facciale o un'impronta digitale, se disponibile. Se vuoi veramente disabilitare l'accesso sicuro, vedi le istruzioni "Accedi automaticamente a Windows 10" di seguito.

**Proteggere le alternative di Windows Hello alla password dell'account**

Vai a **Impostazioni > account > opzioni di** accesso (o fai clic [qui](ms-settings:signinoptions?activationSource=GetHelp)). Verranno elencate le opzioni di accesso disponibili. Ad esempio:

![Opzioni di accesso.](media/sign-in-options.png)

Tocca o fai clic su una delle opzioni per configurarlo. Al successivo avvio o sblocco di Windows, potrai usare la nuova opzione anziché una password. 

**Accedi automaticamente a Windows 10**

**Nota:** l'accesso automatico è pratico, ma introduce un rischio per la sicurezza, soprattutto se il PC è accessibile da più persone. 

1. Tocca o fai clic sul **pulsante Start** nella barra delle applicazioni.

2. Digitare **netplwiz** e premere INVIO per aprire la finestra Account utente.

3. In **Account utente** fare clic sull'account a cui si desidera accedere automaticamente all'avvio di Windows.

4. Deseleziona la casella di controllo "Gli utenti devono immettere un nome utente e una password per usare questo computer".

    ![Gli utenti devono immettere un nome utente e una password.](media/users-must-enter-username.png)

5. Fare clic su **OK**. Verrà richiesto di immettere e confermare la password per l'account selezionato. Fare clic su **OK** per terminare. Al successivo avvio di Windows 10, accederà automaticamente all'account selezionato.
