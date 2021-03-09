---
title: Errore dell'indirizzo proxy durante la creazione di una cassetta postale condivisa
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568294"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Errore dell'indirizzo proxy durante la creazione di una cassetta postale o di un altro oggetto abilitato alla posta elettronica

Se si è tentato di creare un oggetto abilitato alla posta elettronica (cassetta postale, cassetta postale condivisa e così via) e si riceve l'errore "L'indirizzo proxy "SMTP:alias@domain.com" è già in uso...", l'indirizzo di posta elettronica scelto è già stato preso da un altro oggetto abilitato alla posta elettronica nell'organizzazione.
  
È necessario trovare l'utente, il gruppo, la cassetta postale condivisa o la cartella pubblica con questo indirizzo di posta elettronica ed eliminarlo o modificarne l'indirizzo di posta elettronica. È quindi possibile creare un nuovo oggetto abilitato alla posta elettronica con l'indirizzo di posta elettronica liberato. Utilizzare La ricerca nella home page per trovarla. È inoltre possibile utilizzare il seguente comando di PowerShell di Exchange Online per cercarlo:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Se non si desidera eliminare l'indirizzo di posta elettronica esistente, scegliere un nuovo indirizzo di posta elettronica per il nuovo oggetto che si sta creando.
  