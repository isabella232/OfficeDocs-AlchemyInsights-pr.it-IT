---
title: Crittografia con le regole di trasporto
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
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784347"
---
# <a name="encryption-with-transport-rules"></a>Crittografia con le regole di trasporto

Nell'[interfaccia di amministrazione di Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) è possibile usare le funzionalità di Crittografia messaggi di Office nelle regole del flusso di posta per attivare la crittografia dei messaggi. Scegliere l'opzione **Applica Office 365 Message Encryption e la protezione tramite diritti** nella condizione della regola di trasporto.

- Per ulteriori informazioni, vedere [Definire la regola del flusso di posta per la crittografia](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- In PowerShell usare il cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) e impostare il parametro *ApplyOME* su $true.
