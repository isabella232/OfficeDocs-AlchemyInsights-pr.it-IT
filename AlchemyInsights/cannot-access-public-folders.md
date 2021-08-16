---
title: Impossibile accedere alle cartelle pubbliche
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
- "3500007"
- "3462"
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996634"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook non è possibile connettersi alle cartelle pubbliche

Se l'accesso alle cartelle pubbliche non funziona per alcuni utenti, provare a eseguire le operazioni seguenti:

Connessione a EXO PowerShell e configurare il parametro DefaultPublicFolderMailbox nell'account utente problematico in modo che corrisponda al parametro in un account utente funzionante.

Esempio:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Attendere almeno un'ora per l'applicazione della modifica.

Se il problema persiste, seguire [questa procedura per](https://aka.ms/pfcte) risolvere i problemi di accesso alle cartelle pubbliche Outlook.
 
**Per controllare quali utenti possono accedere alle cartelle pubbliche utilizzando Outlook:**

1.  Utilizzare Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true o $false  
      
    $true: consente agli utenti di accedere alle cartelle pubbliche in Outlook  
      
    $false: consente agli utenti di accedere alle cartelle pubbliche in Outlook.  Questo è il valore predefinito.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Nota** Questa procedura può controllare le connessioni solo con Outlook desktop per Windows client. Un utente può continuare ad accedere alle cartelle pubbliche OWA o Outlook per Mac.
 
Per altre info, vedi Annuncio del supporto per le [connessioni controllate alle cartelle](https://aka.ms/controlpf)pubbliche in Outlook .