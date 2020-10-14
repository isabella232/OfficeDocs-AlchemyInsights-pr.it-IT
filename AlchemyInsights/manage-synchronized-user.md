---
title: Gestione degli utenti sincronizzati
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451404"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="e78f1-102">Impossibile impostare l'indirizzo di posta elettronica principale, modificare gli attributi degli utenti o rimuovere/eliminare un utente sincronizzato</span><span class="sxs-lookup"><span data-stu-id="e78f1-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="e78f1-103">Se la sincronizzazione della directory è abilitata per l'ambiente, non è possibile modificare gli attributi di un utente o di un oggetto utilizzando l'interfaccia di amministrazione di Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e78f1-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="e78f1-104">Per gestire completamente gli utenti sincronizzati e tutti gli attributi, utilizzare la console di gestione di utenti e gruppi di Active Directory locale (ADSIEdit. msc).</span><span class="sxs-lookup"><span data-stu-id="e78f1-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="e78f1-105">In alternativa, è possibile modificare singoli utenti o attributi per gli utenti sincronizzati tramite PowerShell, come illustrato negli esempi comuni seguenti:</span><span class="sxs-lookup"><span data-stu-id="e78f1-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
