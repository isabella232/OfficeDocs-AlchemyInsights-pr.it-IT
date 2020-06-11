---
title: Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365
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
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580661"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365

È possibile cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 tramite l'interfaccia di amministrazione. Basta selezionare il gruppo e poi selezionare @modifica indirizzo di posta elettronica.

È anche possibile usare il comando EXO PowerShell per cambiare l'indirizzo SMTP principale di un gruppo di Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Esempio:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
