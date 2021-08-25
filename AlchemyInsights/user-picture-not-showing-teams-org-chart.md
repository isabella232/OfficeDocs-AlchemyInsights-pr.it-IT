---
title: Immagine utente non visualizzata nell'organigramma di Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 08/23/2021
ms.locfileid: "58467378"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Immagine utente non visualizzata nell'organigramma di Microsoft Teams

Se una o più persone dell'organizzazione non hanno la foto del profilo nell'organigramma, è possibile che l'impostazione **ShowInAddressLists** sia impostata su **False**:

1. Andare a interfaccia di amministrazione di Microsoft 365 > [**Utenti attivi**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)e selezionare l'utente con la foto mancante. 
1. Selezionare la scheda **Posta** e verificare che l'opzione **Mostra nell'elenco indirizzi globale** sia impostata su **Sì.** 

Se **l'impostazione di ShowInAddressLists** su **Sì** non funziona, verificare quanto segue:

- L'utente potrebbe essere nascosto dall'elenco dei destinatari in Exchange. Per altre informazioni, vedere [Gestire gli elenchi di indirizzi in Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- L'utente potrebbe essere nascosto dall'elenco indirizzi in Azure Active Directory. Per altre info, vedere [Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 
