---
title: Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 o Microsoft Teams
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756561"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 o Microsoft Teams

È possibile cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 o Microsoft Teams tramite l'[interfaccia di amministrazione di Microsoft 365](https://admin.microsoft.com/). Basta selezionare il gruppo e poi selezionare @modifica indirizzo di posta elettronica.

È anche possibile usare il comando EXO PowerShell seguente per cambiare l'indirizzo SMTP principale di un gruppo di Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Esempio:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
