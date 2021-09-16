---
title: L'immagine dell'utente viene ancora visualizzata nell'organigramma di Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: it-IT
ms.lasthandoff: 09/15/2021
ms.locfileid: "59334383"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>L'immagine dell'utente viene ancora visualizzata nell'organigramma di Microsoft Teams

Se una o più persone dell'organizzazione sono state disabilitate o rimosse e la loro foto del profilo viene ancora visualizzata nell'organigramma, è possibile che l'impostazione **ShowInAddressLists** sia impostata su False: 

1. Aprire l'interfaccia di amministrazione di Microsoft 365 > [Utenti attivi](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) e selezionare l'utente la cui foto viene ancora visualizzata. 
1. Selezionare la scheda **Posta** e verificare che l'opzione **Mostra nell'elenco indirizzi globale** sia impostata su **No**.

Se l'impostazione di **ShowInAddressLists** su **No** non funziona, verificare quanto segue: 

- L'utente potrebbe essere visualizzato dall'elenco destinatari in Exchange. Per altre informazioni, vedere [Gestire gli elenchi di indirizzi in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- L'utente potrebbe essere visualizzato dall'elenco indirizzi in Azure Active Directory. Per altre info, vedere [Set-AzureADUser.](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0) 