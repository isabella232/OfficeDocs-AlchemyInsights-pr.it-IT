---
title: Gestire l'utente sincronizzato
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
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114782"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Impossibile impostare l'indirizzo di posta elettronica principale, modificare gli attributi utente o rimuovere/eliminare un utente sincronizzato

Se la sincronizzazione della directory è abilitata per l'ambiente, alcuni attributi utente o oggetto non possono essere modificati utilizzando il interfaccia di amministrazione di Microsoft 365.

Per gestire completamente gli utenti sincronizzati e tutti i relativi attributi, utilizzare la console di gestione utenti e gruppi di Active Directory locale (adsiedit.msc).  

In alternativa, è possibile modificare singoli utenti o attributi per gli utenti sincronizzati tramite PowerShell, come illustrato negli esempi comuni seguenti:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
