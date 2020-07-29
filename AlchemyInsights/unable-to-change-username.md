---
title: Impossibile modificare il nome utente
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431745"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="0a0bc-102">Impossibile modificare il nome utente</span><span class="sxs-lookup"><span data-stu-id="0a0bc-102">Unable to change UserName</span></span>

<span data-ttu-id="0a0bc-103">In alcuni casi, le modifiche UPN (UserPrincipalName) non verranno propagate nel cloud.</span><span class="sxs-lookup"><span data-stu-id="0a0bc-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="0a0bc-104">Potrebbe essere visualizzato un errore di convalida nel portale di Office 365, oppure potrebbe non essere possibile modificare il nome utente o l'indirizzo di posta elettronica.</span><span class="sxs-lookup"><span data-stu-id="0a0bc-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="0a0bc-105">Per risolvere il problema, impostare manualmente UserPrincipalName con il comando di PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0a0bc-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="0a0bc-106">**Esempio: rinominare un utente**</span><span class="sxs-lookup"><span data-stu-id="0a0bc-106">**Example: Rename a user**</span></span>

<span data-ttu-id="0a0bc-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="0a0bc-107">PowerShellCopy</span></span>

<span data-ttu-id="0a0bc-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="0a0bc-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="0a0bc-109">Questo comando Rinomina davidc@contoso.com in davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="0a0bc-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="0a0bc-110">Per altre informazioni, vedere [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="0a0bc-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>