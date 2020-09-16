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
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733691"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="218e7-102">Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="218e7-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="218e7-103">È possibile cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 tramite l'interfaccia di amministrazione.</span><span class="sxs-lookup"><span data-stu-id="218e7-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="218e7-104">Basta selezionare il gruppo e poi selezionare @modifica indirizzo di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="218e7-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="218e7-105">È anche possibile usare il comando EXO PowerShell per cambiare l'indirizzo SMTP principale di un gruppo di Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="218e7-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="218e7-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="218e7-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="218e7-107">Esempio:</span><span class="sxs-lookup"><span data-stu-id="218e7-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
