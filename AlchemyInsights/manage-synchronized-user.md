---
title: Gestione degli utenti sincronizzati
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
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777681"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Impossibile impostare l'indirizzo di posta elettronica principale, modificare gli attributi degli utenti o rimuovere/eliminare un utente sincronizzato

Se la sincronizzazione della directory è abilitata per l'ambiente, non è possibile modificare gli attributi di un utente o di un oggetto utilizzando l'interfaccia di amministrazione di Microsoft 365.

Per gestire completamente gli utenti sincronizzati e tutti gli attributi, utilizzare la console di gestione di utenti e gruppi di Active Directory locale (ADSIEdit. msc).  

In alternativa, è possibile modificare singoli utenti o attributi per gli utenti sincronizzati tramite PowerShell, come illustrato negli esempi comuni seguenti: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
