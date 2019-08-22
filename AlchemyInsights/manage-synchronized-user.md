---
title: Gestione degli utenti sincronizzati
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542000"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Impossibile impostare l'indirizzo di posta elettronica principale o modificare gli attributi dell'utente

Se la sincronizzazione della directory è abilitata per l'ambiente, non è possibile modificare gli attributi di un utente o di un oggetto utilizzando l'interfaccia di amministrazione di Microsoft 365.

Per gestire completamente gli utenti sincronizzati e tutti gli attributi, utilizzare la console di gestione di utenti e gruppi di Active Directory locale (ADSIEdit. msc).  

In alternativa, è possibile modificare singoli utenti o attributi per gli utenti sincronizzati tramite PowerShell, come illustrato negli esempi comuni seguenti: 
- Set-MsolUser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-title "Manager"-Department "HR"
- Remove-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com