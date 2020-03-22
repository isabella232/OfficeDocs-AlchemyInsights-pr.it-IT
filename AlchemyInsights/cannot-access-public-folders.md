---
title: Non è possibile accedere alle cartelle pubbliche
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891753"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook non è in grado di connettersi alle cartelle pubbliche

Se l'accesso alle cartelle pubbliche non funziona per alcuni utenti, provare a eseguire le operazioni seguenti:

Connettersi a EXO PowerShell e configurare il parametro DefaultPublicFolderMailbox nell'account utente problema in modo che corrisponda al parametro su un account utente funzionante.

Esempio:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<valore dal comando precedente>

Attendere almeno un'ora per rendere effettive le modifiche.

Se il problema persiste, eseguire la [procedura seguente](https://aka.ms/pfcte) per risolvere i problemi di accesso alle cartelle pubbliche con Outlook.