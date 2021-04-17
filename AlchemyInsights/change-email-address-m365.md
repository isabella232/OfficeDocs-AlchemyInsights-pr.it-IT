---
title: Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 o Microsoft Teams
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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819084"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="e12c2-102">Cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e12c2-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="e12c2-103">È possibile cambiare l'indirizzo di posta elettronica di un gruppo di Microsoft 365 o Microsoft Teams tramite l'[interfaccia di amministrazione di Microsoft 365](https://admin.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="e12c2-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="e12c2-104">Basta selezionare il gruppo e poi selezionare @modifica indirizzo di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="e12c2-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="e12c2-105">È anche possibile usare il comando EXO PowerShell seguente per cambiare l'indirizzo SMTP principale di un gruppo di Microsoft 365/Teams:</span><span class="sxs-lookup"><span data-stu-id="e12c2-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="e12c2-106">Esempio:</span><span class="sxs-lookup"><span data-stu-id="e12c2-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
