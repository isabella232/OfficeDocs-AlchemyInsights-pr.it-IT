---
title: Controllare l'accesso alle cartelle pubbliche con Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032562"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controllare l'accesso alle cartelle pubbliche con Outlook

Per controllare quali utenti possono accedere alle cartelle pubbliche con Outlook:

1. Usare `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: consente agli utenti di accedere alle cartelle pubbliche in Outlook  
$false: consente agli utenti di accedere alle cartelle pubbliche in Outlook.  Questo è il valore predefinito.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Nota: questa procedura può solo controllare le connessioni con i client desktop di Outlook per Windows. Gli utenti possono continuare ad accedere alle cartelle pubbliche con OWA o Outlook per Mac.

Per altre informazioni, vedere [Connessioni controllate per le cartelle pubbliche di Outlook](https://aka.ms/controlpf).
