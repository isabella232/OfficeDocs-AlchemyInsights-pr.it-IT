---
title: Micro ritardi o limitazione in PowerShell per Exchange Online
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
- "3500011"
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743918"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro ritardi o limitazione in PowerShell per Exchange Online

Durante l'esecuzione di script e cmdlet in Exchange Online potrebbero verificarsi ritardi o potrebbero comparire avvisi "Applicato micro ritardo". Ecco due suggerimenti a questo proposito:

- Provare a usare il [modulo PowerShell per Exchange Online v2](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), che include CMDlet basati sull'API REST e nettamente più performanti. Può essere un'ottima soluzione per molti CMDlet Get che vengono usati di frequente.
- Se è necessario usare CMDlet non ancora coperti dal modulo v2, vedere l'argomento relativo all'[esecuzione di cmdlet di PowerShell per un numero elevato di utenti in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), che illustra come ovviare ai limiti previsti di PowerShell in Exchange Online.
