---
title: Impossibile modificare il nome utente
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 3088a7b939e7b88319ff688ea94fa71d7fa540787cde31cfd864551113caf149
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020232"
---
# <a name="unable-to-change-username"></a>Impossibile modificare il nome utente

In alcuni casi, le modifiche UPN (UserPrincipalName) non verranno propagate nel cloud. Potrebbe essere visualizzato un errore di convalida nel portale di Office 365, oppure potrebbe non essere possibile modificare il nome utente o l'indirizzo di posta elettronica. Per risolvere il problema, impostare manualmente UserPrincipalName con il comando di PowerShell.

**Esempio: rinominare un utente**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Questo comando Rinomina davidc@contoso.com in davidchew@contoso.com.

Per altre informazioni, vedere [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).