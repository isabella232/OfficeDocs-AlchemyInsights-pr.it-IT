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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282351"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="7e723-102">Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7e723-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="7e723-103">È possibile cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 tramite l'interfaccia di amministrazione.</span><span class="sxs-lookup"><span data-stu-id="7e723-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="7e723-104">Basta selezionare il gruppo e poi selezionare @modifica indirizzo di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="7e723-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="7e723-105">È anche possibile usare il comando EXO PowerShell per cambiare l'indirizzo SMTP principale di un gruppo di Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="7e723-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="7e723-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="7e723-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="7e723-107">Esempio:</span><span class="sxs-lookup"><span data-stu-id="7e723-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
