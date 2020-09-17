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
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798668"
---
# <a name="unable-to-change-username"></a>Impossibile modificare il nome utente

In alcuni casi, le modifiche UPN (UserPrincipalName) non verranno propagate nel cloud. Potrebbe essere visualizzato un errore di convalida nel portale di Office 365, oppure potrebbe non essere possibile modificare il nome utente o l'indirizzo di posta elettronica. Per risolvere il problema, impostare manualmente UserPrincipalName con il comando di PowerShell.

**Esempio: rinominare un utente**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Questo comando Rinomina davidc@contoso.com in davidchew@contoso.com.

Per altre informazioni, vedere [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).