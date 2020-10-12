---
title: Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365
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
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416696"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365

È possibile cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 tramite l'interfaccia di amministrazione. Basta selezionare il gruppo e poi selezionare @modifica indirizzo di posta elettronica.

È anche possibile usare il comando EXO PowerShell per cambiare l'indirizzo SMTP principale di un gruppo di Microsoft 365:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Esempio:

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
