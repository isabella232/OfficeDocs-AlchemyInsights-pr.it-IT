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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816744"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Controllare l'accesso alle cartelle pubbliche con Outlook

Per controllare quali utenti possono accedere alle cartelle pubbliche con Outlook:

1. Usare `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: consente agli utenti di accedere alle cartelle pubbliche in Outlook  
$false: consente agli utenti di accedere alle cartelle pubbliche in Outlook.  Questo è il valore predefinito.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Nota: questa procedura può solo controllare le connessioni con i client desktop di Outlook per Windows. Gli utenti possono continuare ad accedere alle cartelle pubbliche con OWA o Outlook per Mac.

Per altre informazioni, vedere [Connessioni controllate per le cartelle pubbliche di Outlook](https://aka.ms/controlpf).
