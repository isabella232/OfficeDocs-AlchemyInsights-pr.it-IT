---
title: Modificare il requisito di password complessa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818472"
---
# <a name="change-strong-password-requirement"></a>Modificare il requisito di password complessa

Microsoft richiede password complesse per impostazione predefinita.

Usando PowerShell, è possibile disabilitare password complesse per utenti specifici con questi comandi:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Per disabilitare password complesse per tutti gli utenti, utilizzare:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Ulteriori informazioni sui criteri password](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Come connettersi a Microsoft 365 con PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Ulteriori informazioni sui comandi MsolUser di PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
