---
title: Controllare l'accesso alle cartelle pubbliche con Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: b04e09f5110266d59db82e25cfda1835779fd4b7
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406581"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controllare l'accesso alle cartelle pubbliche con Outlook

Per controllare quali utenti possono accedere alle cartelle pubbliche con Outlook:

1. Usare `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: consente agli utenti di accedere alle cartelle pubbliche in Outlook  
$false: consente agli utenti di accedere alle cartelle pubbliche in Outlook.  Questo è il valore predefinito.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Nota: questa procedura può solo controllare le connessioni con i client desktop di Outlook per Windows. Gli utenti possono continuare ad accedere alle cartelle pubbliche con OWA o Outlook per Mac.

Per altre informazioni, vedere [Connessioni controllate per le cartelle pubbliche di Outlook](https://aka.ms/controlpf).
