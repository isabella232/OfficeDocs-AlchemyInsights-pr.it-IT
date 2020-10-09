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
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="9ebed-102">Cartella pubblica abilitata alla posta elettronica Senda</span><span class="sxs-lookup"><span data-stu-id="9ebed-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="9ebed-103">Nell'esempio seguente vengono assegnate le autorizzazioni "Invia come" per la cartella pubblica abilitata alla posta NewPF1 all'utente Jason.</span><span class="sxs-lookup"><span data-stu-id="9ebed-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="9ebed-104">Add-RecipientPermission-Identity ' NewPF1'-trustee "Jason"-AccessRights ' Senda '</span><span class="sxs-lookup"><span data-stu-id="9ebed-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="9ebed-105">Per informazioni dettagliate sulla sintassi e sui parametri, vedere [assegnare le autorizzazioni "Invia come" o "Invia per conto di" per le cartelle pubbliche abilitate alla posta elettronica](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="9ebed-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>
