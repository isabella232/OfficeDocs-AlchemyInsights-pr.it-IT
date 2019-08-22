---
title: Gestione degli utenti sincronizzati
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542000"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="e6a80-102">Impossibile impostare l'indirizzo di posta elettronica principale o modificare gli attributi dell'utente</span><span class="sxs-lookup"><span data-stu-id="e6a80-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="e6a80-103">Se la sincronizzazione della directory è abilitata per l'ambiente, non è possibile modificare gli attributi di un utente o di un oggetto utilizzando l'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e6a80-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="e6a80-104">Per gestire completamente gli utenti sincronizzati e tutti gli attributi, utilizzare la console di gestione di utenti e gruppi di Active Directory locale (ADSIEdit. msc).</span><span class="sxs-lookup"><span data-stu-id="e6a80-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="e6a80-105">In alternativa, è possibile modificare singoli utenti o attributi per gli utenti sincronizzati tramite PowerShell, come illustrato negli esempi comuni seguenti:</span><span class="sxs-lookup"><span data-stu-id="e6a80-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="e6a80-106">Set-MsolUser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e6a80-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="e6a80-107">Set-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-title "Manager"-Department "HR"</span><span class="sxs-lookup"><span data-stu-id="e6a80-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="e6a80-108">Remove-MsolUser-UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="e6a80-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>