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
# <a name="unable-to-change-username"></a>Impossibile modificare il nome utente

In alcuni casi, le modifiche UPN (UserPrincipalName) non verranno propagate nel cloud. Potrebbe essere visualizzato un errore di convalida nel portale di Office 365, oppure potrebbe non essere possibile modificare il nome utente o l'indirizzo di posta elettronica. Per risolvere il problema, impostare manualmente UserPrincipalName con il comando di PowerShell.

**Esempio: rinominare un utente**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Questo comando Rinomina davidc@contoso.com in davidchew@contoso.com.

Per altre informazioni, vedere [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).