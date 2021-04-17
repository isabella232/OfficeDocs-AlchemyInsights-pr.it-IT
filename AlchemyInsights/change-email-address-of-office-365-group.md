---
title: Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365
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
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819048"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365

È possibile cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 tramite l'interfaccia di amministrazione. Basta selezionare il gruppo e poi selezionare @modifica indirizzo di posta elettronica.

È anche possibile usare il comando EXO PowerShell per cambiare l'indirizzo SMTP principale di un gruppo di Microsoft 365:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Esempio:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
