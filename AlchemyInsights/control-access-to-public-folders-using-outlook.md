---
title: Controllare l'accesso alle cartelle pubbliche con Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680486"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controllare l'accesso alle cartelle pubbliche con Outlook

Per controllare quali utenti possono accedere alle cartelle pubbliche con Outlook:

1. Usare `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: consente agli utenti di accedere alle cartelle pubbliche in Outlook  
$false: consente agli utenti di accedere alle cartelle pubbliche in Outlook.  Questo è il valore predefinito.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Nota: questa procedura può solo controllare le connessioni con i client desktop di Outlook per Windows. Gli utenti possono continuare ad accedere alle cartelle pubbliche con OWA o Outlook per Mac.

Per altre informazioni, vedere [Connessioni controllate per le cartelle pubbliche di Outlook](https://aka.ms/controlpf).
