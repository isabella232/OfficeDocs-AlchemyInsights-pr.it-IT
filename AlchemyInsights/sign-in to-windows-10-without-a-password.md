---
title: Accedere a un Windows 10 senza usare una password
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
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107523"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Accedere a un Windows 10 senza usare una password

Per evitare di dover digitare una password all'avvio di Windows, ti consigliamo di usare una delle opzioni di accesso sicuro di Windows Hello, ad esempio un PIN, un riconoscimento del volto o un'impronta digitale, se disponibile. Se vuoi veramente disabilitare l'accesso sicuro, vedi le istruzioni "Accedi automaticamente a Windows 10" di seguito.

**Proteggere Windows Hello alternative alla password dell'account**

Vai a **Impostazioni > account > opzioni di accesso** (o fai clic [qui](ms-settings:signinoptions?activationSource=GetHelp)). Verranno elencate le opzioni di accesso disponibili. Ad esempio:

![Opzioni di accesso.](media/sign-in-options.png)

Tocca o fai clic su una delle opzioni per configurarlo. Al successivo avvio o sblocco Windows, sarà possibile utilizzare la nuova opzione anziché una password. 

**Accedi automaticamente a Windows 10**

**Nota:** l'accesso automatico è pratico, ma introduce un rischio per la sicurezza, soprattutto se il PC è accessibile da più persone. 

1. Tocca o fai clic sul **pulsante Start** nella barra delle applicazioni.

2. Digitare **netplwiz** e premere INVIO per aprire la finestra Account utente.

3. In **Account utente** fare clic sull'account a cui si desidera accedere automaticamente all'Windows avvio.

4. Deseleziona la casella di controllo "Gli utenti devono immettere un nome utente e una password per usare questo computer".

    ![Gli utenti devono immettere un nome utente e una password.](media/users-must-enter-username.png)

5. Fare clic su **OK**. Verrà richiesto di immettere e confermare la password per l'account selezionato. Fare clic su **OK** per terminare. Al successivo Windows 10, accederà automaticamente all'account selezionato.
