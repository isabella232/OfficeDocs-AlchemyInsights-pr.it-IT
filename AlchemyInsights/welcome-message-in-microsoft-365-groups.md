---
title: Messaggio di benvenuto nei Gruppi di Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 05/19/2020
ms.locfileid: "44320461"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Messaggio di benvenuto nei Gruppi di Microsoft 365

I nuovi utenti che partecipano al gruppo di Microsoft 365 riceveranno un messaggio di benvenuto se la proprietà "UnifiedGroupWelcomeMessageEnabled" è impostata su Vero.

Nel caso si voglia disabilitare il messaggio di benvenuto, usare il comando [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) seguente:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
