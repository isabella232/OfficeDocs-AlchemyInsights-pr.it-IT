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
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819516"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook non è in grado di connettersi alle cartelle pubbliche

Se l'accesso alle cartelle pubbliche non funziona per alcuni utenti, provare a eseguire le operazioni seguenti:

Connettersi a EXO PowerShell e configurare il parametro DefaultPublicFolderMailbox nell'account utente problematico in modo che corrisponda al parametro in un account utente funzionante.

Esempio:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Attendere almeno un'ora per l'applicazione della modifica.

Se il problema persiste, seguire [questa procedura per](https://aka.ms/pfcte) risolvere i problemi di accesso alle cartelle pubbliche tramite Outlook.
 
**Per controllare quali utenti possono accedere alle cartelle pubbliche tramite Outlook:**

1.  Utilizzare Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true o $false  
      
    $true: consente agli utenti di accedere alle cartelle pubbliche in Outlook  
      
    $false: consente agli utenti di accedere alle cartelle pubbliche in Outlook.  Questo è il valore predefinito.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Nota** Questa procedura consente di controllare le connessioni solo con il desktop di Outlook per i client Windows. Un utente può continuare ad accedere alle cartelle pubbliche OWA o Outlook per Mac.
 
Per ulteriori informazioni, vedere Annuncio del supporto per le [connessioni controllate alle cartelle pubbliche in Outlook.](https://aka.ms/controlpf)