---
title: Accedere a Windows 10 senza utilizzare una password
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719957"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Accedere a Windows 10 senza utilizzare una password

Per evitare di dover digitare una password all'avvio di Windows, si consiglia di utilizzare una delle opzioni di accesso sicuro di Windows Hello, come un PIN, il riconoscimento del volto o l'impronta digitale, se disponibile. Se si vuole davvero disabilitare l'accesso sicuro, vedere le istruzioni "Accedi automaticamente a Windows 10" di seguito.

**Protezione delle alternative di Windows Hello per la password dell'account**

Andare a **impostazioni > account > opzioni di accesso** (o fare clic [qui](ms-settings:signinoptions?activationSource=GetHelp)). Vengono elencate le opzioni di accesso disponibili. Ad esempio:

![Opzioni di accesso.](media/sign-in-options.png)

Fare clic o toccare una delle opzioni per configurarla. La volta successiva che si avvia o si sblocca Windows, è possibile utilizzare la nuova opzione invece di una password. 

**Accesso automatico a Windows 10**

**Nota**: l'accesso automatico è comodo, ma introduce un rischio per la sicurezza, soprattutto se il PC è accessibile da più persone. 

1. Fare clic o toccare il pulsante **Start** nella barra delle applicazioni.

2. Digitare **Netplwiz** e premere INVIO per aprire la finestra account utente.

3. In **account utente**, fare clic sull'account che si desidera accedere automaticamente al momento dell'avvio di Windows.

4. Deselezionare la casella di controllo "gli utenti devono immettere un nome utente e una password per l'utilizzo del computer".

    ![Gli utenti devono immettere l'opzione nome utente e password.](media/users-must-enter-username.png)

5. Fare clic su **OK**. Verrà chiesto di immettere e confermare la password per l'account selezionato. Fare clic su **OK** per terminare. La volta successiva che viene avviato Windows 10, l'utente accede automaticamente all'account selezionato.
