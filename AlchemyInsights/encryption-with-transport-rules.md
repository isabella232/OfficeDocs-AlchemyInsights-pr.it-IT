---
title: Crittografia con le regole di trasporto
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
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079454"
---
# <a name="encryption-with-transport-rules"></a>Crittografia con le regole di trasporto

Nell'[interfaccia di amministrazione di Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) è possibile usare le funzionalità di Crittografia messaggi di Office nelle regole del flusso di posta per attivare la crittografia dei messaggi. Scegliere l'opzione **Applica Office 365 Message Encryption e la protezione tramite diritti** nella condizione della regola di trasporto.

- Per ulteriori informazioni, vedere [Definire la regola del flusso di posta per la crittografia](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- In PowerShell usare il cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) e impostare il parametro *ApplyOME* su $true.
