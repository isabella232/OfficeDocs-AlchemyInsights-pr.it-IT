---
title: Invia come cartella pubblica abilitata alla posta elettronica in EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 0765262c04571e7df139de993611fd6e67068c54
ms.sourcegitcommit: 45635cc7a6c36d6c7b5f78215ad32f2aa7e3aed0
ms.translationtype: MT
ms.contentlocale: it-IT
ms.lasthandoff: 10/08/2020
ms.locfileid: "48394689"
---
# <a name="sendas-mail-enabled-public-folder"></a>Cartella pubblica abilitata alla posta elettronica Senda

Nell'esempio seguente vengono assegnate le autorizzazioni "Invia come" per la cartella pubblica abilitata alla posta NewPF1 all'utente Jason.

Add-RecipientPermission-Identity ' NewPF1'-trustee "Jason"-AccessRights ' Senda '

Per informazioni dettagliate sulla sintassi e sui parametri, vedere [assegnare le autorizzazioni "Invia come" o "Invia per conto di" per le cartelle pubbliche abilitate alla posta elettronica](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).
