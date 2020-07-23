---
title: Exchange PowerShell e deprecazione dell'autenticazione di base
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: a0f01d7ecaa444777aa0675795e588790ab22f19
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/22/2020
ms.locfileid: "45205199"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a>Exchange PowerShell e deprecazione dell'autenticazione di base

Per le informazioni più recenti riguardanti le modalità di connessione Exchange Online PowerShell senza l'uso dell'autenticazione di base, [fare clic qui](https://aka.ms/exops-docs). Il modulo di PowerShell V2 non usa l'autenticazione di base.

Tenere presente che l'autenticazione di base deve comunque essere abilitata nel computer client.
Il nuovo modulo PowerShell V2 usa l'autenticazione moderna per stabilire una connessione per l'abilitazione di tutti i cmdlet V2 basati su REST. Oltre ai cmdlet V2, consente anche di accedere ai cmdlet di PowerShell remoto (RPS) meno recenti, per cui è necessario stabilire una sessione PowerShell remota. Per stabilire una sessione RPS in un computer Windows, è necessario abilitare WinRM BasicAuth nel computer client anche se il modulo usa il meccanismo di autenticazione moderna per l'autenticazione nel servizio. La pipeline di autenticazione di base WinRM consente di trasportare i token di autenticazione moderna. Se l'autenticazione di base WinRM è disabilitata nel computer client, i nuovi cmdlet V2 continueranno a funzionare, ma i cmdlet RPS meno recenti non funzioneranno più.
