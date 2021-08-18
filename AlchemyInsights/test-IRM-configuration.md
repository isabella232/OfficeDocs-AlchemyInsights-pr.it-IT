---
title: Testare la configurazione IRM per le nuove funzionalità di OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 22430e2b8a00023f9922fd59d6fcabd308d08453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317236"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Testare la configurazione IRM per le nuove funzionalità di OME

Per verificare se il tenant di Microsoft 365 è configurato per l'uso delle nuove funzionalità di OME, eseguire i cmdlet seguenti mentre è connesso a [PowerShell di Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell):


1. Controllare la configurazione IRM del tenant eseguendo `Get-IRMConfiguration`. Assicurarsi che questi valori siano impostati su **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Usando il dominio, l'indirizzo del mittente e il destinatario, eseguire `Test-IRMConfiguration`. Se il test non viene superato, esaminare la configurazione IRM.

Per altre informazioni su come verificare la configurazione di IRM, vedere [Verificare la nuova configurazione di OME in PowerShell di Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).