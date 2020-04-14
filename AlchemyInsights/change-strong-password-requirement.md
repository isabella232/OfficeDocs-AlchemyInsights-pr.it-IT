---
title: Modificare i requisiti per la password complessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286267"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="3e315-102">Modificare i requisiti per la password complessa</span><span class="sxs-lookup"><span data-stu-id="3e315-102">Change strong password requirement</span></span>

<span data-ttu-id="3e315-103">Microsoft richiede password complesse per impostazione predefinita.</span><span class="sxs-lookup"><span data-stu-id="3e315-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="3e315-104">Tramite PowerShell, è possibile disabilitare password complesse per utenti specifici con questo comando:</span><span class="sxs-lookup"><span data-stu-id="3e315-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="3e315-105">*Set-MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="3e315-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="3e315-106">Ulteriori informazioni sui criteri password</span><span class="sxs-lookup"><span data-stu-id="3e315-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="3e315-107">Come connettersi a Office 365 con PowerShell</span><span class="sxs-lookup"><span data-stu-id="3e315-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="3e315-108">Ulteriori informazioni sui comandi di MsolUser di PowerShell</span><span class="sxs-lookup"><span data-stu-id="3e315-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [<span data-ttu-id="3e315-109">Impostare la password di un singolo utente in modo che non scada mai</span><span class="sxs-lookup"><span data-stu-id="3e315-109">Set an individual user's password to never expire</span></span>](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
