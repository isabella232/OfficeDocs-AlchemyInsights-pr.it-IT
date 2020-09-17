---
title: Non è possibile accedere alle cartelle pubbliche
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
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812551"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook non è in grado di connettersi alle cartelle pubbliche

Se l'accesso alle cartelle pubbliche non funziona per alcuni utenti, provare a eseguire le operazioni seguenti:

Connettersi a EXO PowerShell e configurare il parametro DefaultPublicFolderMailbox nell'account utente problema in modo che corrisponda al parametro su un account utente funzionante.

Esempio:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Attendere almeno un'ora per rendere effettive le modifiche.

Se il problema persiste, eseguire la [procedura seguente](https://aka.ms/pfcte) per risolvere i problemi di accesso alle cartelle pubbliche con Outlook.
 
**Per controllare quali utenti possono accedere alle cartelle pubbliche con Outlook**:

1.  Utilizzare Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true o $false  
      
    $true: consente agli utenti di accedere alle cartelle pubbliche in Outlook  
      
    $false: consente agli utenti di accedere alle cartelle pubbliche in Outlook.  Questo è il valore predefinito.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Note** Questa procedura consente di controllare le connessioni solo con i client di Outlook desktop per Windows. Un utente può continuare ad accedere alle cartelle pubbliche utilizzando OWA o Outlook per Mac.
 
Per altre informazioni, vedere [annuncio del supporto per le connessioni controllate alle cartelle pubbliche in Outlook](https://aka.ms/controlpf).