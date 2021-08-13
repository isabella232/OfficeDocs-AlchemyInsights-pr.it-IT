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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062912"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Errore dell'indirizzo proxy durante la creazione di una cassetta postale o di un altro oggetto abilitato alla posta elettronica

Se si è tentato di creare un oggetto abilitato alla posta elettronica (cassetta postale, cassetta postale condivisa e così via) e si è ricevuto l'errore "L'indirizzo proxy "SMTP:alias@domain.com" è già in uso...", l'indirizzo di posta elettronica scelto è già preso da un altro oggetto abilitato alla posta elettronica nell'organizzazione.
  
È necessario trovare l'utente, il gruppo, la cassetta postale condivisa o la cartella pubblica con questo indirizzo di posta elettronica ed eliminarlo o modificarne l'indirizzo di posta elettronica. È quindi possibile creare un nuovo oggetto abilitato alla posta elettronica con l'indirizzo di posta elettronica liberato. Utilizzare Cerca nella home page per trovarla. È inoltre possibile utilizzare il comando Exchange Online PowerShell seguente per cercarlo:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Se non si desidera eliminare l'indirizzo di posta elettronica esistente, scegliere un nuovo indirizzo di posta elettronica per il nuovo oggetto che si sta creando.
  